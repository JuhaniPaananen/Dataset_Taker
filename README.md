### Dataset_Taker

This is program, that is made to help for taking picture to your dataset.

# Step 1

Create folders named: dataset and labels.
Dataset is for pictures and labels are for validation text files,that contains: Class (number), x_center, y_center, width, height of pictures.

Change class number at line 68 if you want to use different class. Number is before {x_center:.6f}.

=> f.write(f"0 {x_center:.6f} {y_center:.6f} {w_norm:.6f} {h_norm:.6f}\n")

If you want, add count.json, that is made to keep your progress, when making your dataset. It saves the order count, that scrpts adds to files like: Image_23.png and Image_23.txt.
Without json it starts always from 0.

# Step 2

Open application with this command: python Taker.py and your are good to go.

If you press space, it will open a new window.

That window will have picture of moment you pressed space. Now with mouse drag a box around, what you want to train your dataset with. 
Then press space a again to save it. Picture and text file should be in their specific folders.

To quit press Q.

