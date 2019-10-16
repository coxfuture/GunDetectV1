# GunDetectV1
Tensorflow weapon detection module, v1. Trained 200000 steps on Power9 hardware with 2x Nvidia Tesla v100s. Haven't benchmarked it yet, but it appears to be fairly accurate.

This was trained on a hand-tagged dataset of 2,000 images with 7 types of weapons: AR-Type rifle, Ak-type rifle, shotgun, hunting rifle, mp5, pistol, holstered pistol

The recognition between pistol and holstered pistol is spotty, so if the functionality is not required, I'd recommend simply editing your labelmap to detect them both as the same.
MP5 for now will only detect MP5-style submachineguns, but will likely expand to include all submachine guns in a future update

Coming soon is a V2 model, trained for 2M steps on 150,000 images of an augmented dataset. (same pictures, with random transforms and light changes)

Hope someone can get some use out of this!
