
# Foveated Diffusion Through a Neuroscience Lens: Reproducing Mixed-Resolution Generation on a Budget

**Introduction to NeuroAI 02360606 – Final Project, Technion, 2026**

## 👥 Authors
* **Roy Carmel** &  **Roi Maman** 

---

## 📂 Repository Structure

* **`Final_codes.ipynb`**: The main Jupyter Notebook containing the complete implementation, training loops, and evaluation scripts for the foveated generation pipeline.
* **`report.pdf`**: The report in which we have documented our work.
* **`Original_Paper.pdf`**: The original paper on which we based our work
* **`foveated_diffusion.yml`**: Conda environment configuration file. Use this to recreate the exact environment and dependencies required to run the notebook.
* **`example.png`**: A sample generated image demonstrating the outputs of our foveated models.
* **`*.zip` files**: These archives contain the fine-tuned LoRA weights for the different models we trained and evaluated:
  * `pixart_foveated_lora_downsample.zip` & `..._10k_exact.zip`: Weights for the Random-mask LoRA configurations.
  * `pixart_foveated_lora_gabor...zip`: Weights for the Gabor-mask LoRA configurations.

---

## ⚠️ Important Setup Step: Extracting LoRA Weights

Before running the evaluation cells in `Final_codes.ipynb`, you **should extract the pre-trained LoRA weights** from the `.zip` files, so that you won't have to rerun the training code (unless you want to, and then there will be further instruction in the notebook above the training code blocks.). 

Please unzip all the `.zip` archives directly into the root directory of this project. The notebook expects to find the extracted folders containing the model weights in order to load them correctly during the generation process.

---