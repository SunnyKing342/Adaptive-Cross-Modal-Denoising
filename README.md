# Adaptive Cross-Modal Denoising (ACMD)
Official implementation of the paper:
**Adaptive Cross-Modal Denoising: Enhancing LiDAR–Camera Fusion Perception in Adverse Circumstances**

<img width="696" height="237" alt="image" src="https://github.com/user-attachments/assets/44f7cc1c-6cb2-4061-a8be-867f03feabe7" />

---

## About
This repository contains the implementation of a cross-modal denoising framework designed to improve LiDAR–camera fusion perception under adverse conditions (e.g., rain, fog, snow, and low light).

The method introduces an adaptive cross-modal denoising approach that:
- Estimates the reliability of each modality
- Uses the cleaner modality to guide refinement of the noisy one
- Improves overall perception accuracy while maintaining real-time performance

---

## Requirements
- Python ≥ 3.8
- PyTorch ≥ 1.10
- OpenCV
- NumPy
- tqdm
- scikit-learn

Install dependencies:
```bash
pip install -r requirements.txt
```

---

## Usage
1.  **Prepare your dataset** (e.g., adverse-condition LiDAR-camera data following the structure described in the paper).
2.  Run the denoising pipeline:
    ```bash
    python main.py --config config/acmd.yaml --data_path ./data/
    ```
3.  Visualize results:
    ```bash
    python visualize.py --output_path ./results/
    ```

---

## Citation
If you use this code in your research, please cite:

```bibtex
@article{ghaffar2026adaptive,
  title={Adaptive Cross-Modal Denoising: Enhancing LiDAR--Camera Fusion Perception in Adverse Circumstances},
  author={Ghaffar, Muhammad Arslan and Zhang, Kangshuai and Pan, Nuo and Peng, Lei},
  journal={Sensors},
  volume={26},
  number={2},
  pages={408},
  year={2026},
  publisher={MDPI}
}
```

---

## License
This work is licensed under the **CC BY 4.0 License** (consistent with the Sensors (MDPI) open-access policy).

---

## Contact
For questions or issues, please contact:

Muhammad Arslan Ghaffar – ghaffar@siat.ac.cn
