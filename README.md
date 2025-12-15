# Solving the 1d Heat Equation for a variable diffusivity distribution using Fourier Neural Operators

First, I generated training data by solving the Heat equation with a spectral method in `heat1d_data.ipynb`. The dataset is stored in `heat1d_dataset.npy`.

Then, I trained a Fourier Neural Operator on the data in `train_heat1d.ipynb` and saved the model in `heat1d.eqx`.

Finally, I generate a random scenario in `eval_heat1d.ipynb` and evaluate it using the model. I demonstrate zero-shot superresolution by evaluating the model on a 1000-point mesh; it was trained on a 100-point mesh.
