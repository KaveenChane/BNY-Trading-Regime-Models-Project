# BNY-Trading-Regime-Models-Project

## Description
This project aims to develop an algorithm capable of automatically classifying short-term market regimes (1 to 5 minutes) using Wasserstein K-means clustering. The objective is to propose investment strategies adapted to the identified regimes.

## Objectives
- Create a clustering algorithm for FX market regimes.
- Initially use a single variable, then extend to a multivariate model, implementing a Wasserstein K-means model.

## Project Structure
The project contains the following key notebooks:

- `Final_Multivariate_Wasserstein.ipynb` implements multivariate Wasserstein K-means, applied to financial data with log-returns and volatility. It uses sliced Wasserstein distance to measure similarity between multidimensional distributions and segments market regimes through optimized clustering on sliding windows.
  
- `Wasserstein_K_means_V2.ipynb` implements univariate Wasserstein K-means clustering, using sliced Wasserstein distance to measure similarity between time series windows. It applies K-means on Wasserstein distances to segment financial data into distinct market regimes. 

- `README.md` - This file.

## Installation

### Prerequisites
- **Python 3.8+**
- **Jupyter Notebook**
- Required Python libraries:
  ```bash
  pip install numpy pandas scipy scikit-learn matplotlib ot jupyter
  ```
  (The `ot` library refers to **POT** - Python Optimal Transport) 

## Execution

1. **Clone the repository**:
   ```bash
   git clone https://github.com/KaveenChane/BNY-Trading-Regime-Models-Project.git
   cd BNY-Trading-Regime-Models-Project
   ```

2. **Open Jupyter Notebook and run the files**:
   - `Final_Multivariate_Wasserstein.ipynb`

## Contribution

1. **Fork the repository**.
2. **Create a new branch**:
   ```bash
   git checkout -b feature-new-feature
   ```
3. **Add your modifications**:
   ```bash
   git add .
   git commit -m "Added a new feature"
   git push origin feature-new-feature
   ```
4. **Open a Pull Request on GitHub**.

## Credits

Project developed by the BNY Team no. 246 as part of research for the PI² project of our school.

## License

This project is licensed under the **[MIT License](https://opensource.org/licenses/MIT)**.
