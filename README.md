# What?
This is a Python script that writes Git commits into whatever patterns you give it.
I don't believe in error handling, so if you try to use it and it breaks, that's on you.

# How to Use
1. Make sure you run `git init` to initialize an empty repo, or all the git commands from Python will fail
2. Use Paint or Photoshop or whatever to draw a design that fits into a 52x7 image, template provided in `template.png`
3. Update `main.py` to take the path of the image as an argument
4. Run `pip install -r requirements.txt`, or make sure you have `pillow` installed
5. Run `main.py`
6. Add your git remote `git remote add <your_remote_link>` and push `git push --set-upstream origin master`
7. Begin levitating a few inches of the ground due to your now overwhelming intellectual superiority

The script should handle generating the right number of commits on the right days, based on how dark each pixel in the original image is.
I gotta be honest I didn't test this very extensively with anything other than black and white images (no gray values really) so it remains
to be seen if those work very well.

Also you might run into trouble if it's a leap year. See the comment in `main.py`. Good luck!