Inductor and Transformer MDN Models
The models are stored in the branches named ind and trf, respectively.

Models: IND1, IND2, IND5; TRF1, TRF2, TRF3, TRF5, TRF7.
Purpose: predict candidate geometries from the corresponding response representation.

Inputs (before MDN scaling):
ind/trans 6/20 VAE latent vectors from each type's matching VAE.

Outputs:
- IND1/2/5: [Wmax, S, Wmin, N, Din, Ra].
- TRF1/2/3/5/7: 5/5/4/9/9 geometry parameters, respectively.

Environment: Python 3.12, PyTorch, NumPy, scikit-learn, joblib.
Geometry and EMX validation are still required. Weights are unchanged.

Because the models were trained over an extended period, the inductor and transformer model filename suffixes differ, but this does not affect normal loading with their corresponding loaders.
