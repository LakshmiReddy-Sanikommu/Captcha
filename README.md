Image Captcha Verification
This project is an implementation of an image-based CAPTCHA verification system using Python and Tkinter. The user is presented with a 3x3 grid of images and asked to select all images that match a given category (e.g., "Select all images which contain a bird"). The program then verifies whether the user's selections are correct.

Features
Randomly generated set of images from three categories: birds, cakes, and roads.
Dynamically generated CAPTCHA prompt based on a randomly chosen category.
Verifies user selections against the correct answers.
Provides feedback on whether the CAPTCHA was verified successfully or if there was a mismatch.
Prerequisites
Python 3.x
Tkinter (usually included with Python installations)
Pillow (Python Imaging Library Fork)
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/image-captcha-verification.git
cd image-captcha-verification
Install the required packages:

bash
Copy code
pip install pillow
Add your images to the project directory. Ensure the images are named and categorized as per the img_ran dictionary:

python
Copy code
img_ran = { 
    1: "b1.jpg", 2: "b2.jpg", 3: "b3.jpg", 
    4: "c1.jpg", 5: "c2.jpg", 6: "c3.jpg", 
    7: "r1.jpg", 8: "r2.jpg", 9: "r3.jpg"
}
Usage
Run the captcha.py script:

bash
Copy code
python captcha.py
A window will appear with the CAPTCHA prompt and a 3x3 grid of images. Follow these steps:

Read the prompt to know which category of images to select.
Click on the checkboxes below the images that match the given category.
Click the "Verify" button to check your selections.
Based on your selections, you will see one of the following messages:

"Captcha Verified!" if your selections are correct.
"Uh Oh! Captcha Mismatch! Try Again!" if your selections are incorrect.
Code Explanation
The script starts by defining the categories and images.
Random images are selected and displayed in a grid layout.
The user is prompted to select images from a specific category.
A verification function checks the user's selections against the correct answers and provides feedback.
Contributing
If you would like to contribute to this project, please fork the repository and submit a pull request. You can also report issues or suggest features by opening an issue on GitHub.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgments
This project uses the Tkinter library for the GUI and Pillow for image processing.
