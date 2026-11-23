# 🛩️ Foam Glider Wing Aspect Ratio & Repeatability Simulator

An interactive simulation tool I built in Google Colab using **Gradio**, **NumPy**, and **Matplotlib** to compare low, mid, and high wing Aspect Ratios (AR) on foam gliders by looking at glide distance, target landing accuracy, and trial-to-trial repeatability.

## ✨ Key Features
- **Multi-AR Comparison:** Compare three selectable Aspect Ratio configurations (*Low AR*, *Mid AR*, *High AR*) under shared glider mass, wing area, launch height, and launch speed settings.
- **Monte Carlo Trial Simulation:** Models small variations in launch speed, launch angle, and wind gusts across hundreds of virtual tosses to inspect real-world scatter.
- **Accuracy & Repeatability Metrics:** Tracks mean glide distance, standard deviation, absolute error relative to a target landing distance, and a repeatability score.
- **Side-by-Side Visual Output:** Plots glide distance histograms against the target line alongside trial-by-trial landing error curves.

## 🛠️ Tech Stack
- **Environment:** Google Colab (no foam cutting, field tossing setup, or desktop software needed)
- **Simulation & UI:** Python, Gradio, NumPy, Matplotlib

## ⚙️ How to Run the Project
1. **Open in Google Colab:**
   - Upload `foam-glider-aspect-ratio-repeatability.ipynb` to Google Colab (`colab.research.google.com`).
2. **Run & Launch the App:**
   - Run the notebook cells; Gradio will install `gradio`, `matplotlib`, and `numpy` and display the interactive interface right below the cell (plus a temporary `gradio.live` link if desired).
3. **Explore & Iterate:**
   - Adjust Aspect Ratios, launch height/speed, target distance, or trial scatter sliders and click **Simulate Glider Trials** to compare performance trade-offs.

## 📌 Scope & Assumptions
- Built for **conceptual trade-off exploration and repeatability analysis**, not full 6-DOF flight dynamics or physical flight-test certification.
- Uses steady-state induced/parasitic drag trade-offs for nominal glide ratio estimates and Gaussian perturbations to represent launch/gust variability.
