# neural_style_transfer

Neural style transfer with Keras.
Before running this script, download the weights for the VGG16 model at:
https://drive.google.com/file/d/0Bz7KyqmuGsilT0J5dmRCM0ROVHc/view?usp=sharing
(source: https://gist.github.com/baraldilorenzo/07d7802847aaad0a35d3)
and make sure the variable `weights_path` in this script matches the location of the file.
Run the script with:
```
python neural_style_transfer.py path_to_your_base_image.jpg path_to_your_reference.jpg prefix_for_results
```
e.g.:
```
python neural_style_transfer.py img/tuebingen.jpg img/starry_night.jpg results/my_result
```
It is preferable to run this script on GPU, for speed.
If running on CPU, prefer the TensorFlow backend (much faster).
Added some improvements based on "Improving the Neural Algorithm of Artistic Style".

# References
    - [A Neural Algorithm of Artistic Style](http://arxiv.org/abs/1508.06576)
    - [Improving the Neural Algorithm of Artistic Style](https://arxiv.org/abs/1605.04603)
