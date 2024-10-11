````markdown
# Project: Machine Learning-Based SMS Spam Filtering

## Part 1: Instructions to Execute the Code and Generate an ARFF File

### 1. Ensure Required Files are in the Same Directory:

- `smsfiltering.js`
- `english_big.txt`

### 2. Open Working Directory:

- Open the directory where the files are located using Command Prompt or Terminal.

### 3. Node.js Requirement:

- **Ensure Node.js is installed** on your machine to run JavaScript code.

### 4. Skip to Step 6 If Node.js is Installed:

- If Node.js is already installed, proceed directly to step 6.

### 5. Install Node.js:

- **Windows:** Download and install from [Node.js official website](https://nodejs.org/).
- **Linux:** Install via package manager:
  - For Ubuntu/Debian:
    ```bash
    sudo apt update
    sudo apt install nodejs
    ```
  - For Red Hat/CentOS/Fedora:
    ```bash
    sudo yum install nodejs
    ```
  - Install Node Package Manager (npm) as well.
- **macOS:** Use Homebrew to install Node.js:
  ```bash
  brew install node
  ```
````

### 6. Run the Code:

- Navigate to the directory containing the files and execute:
  ```bash
  node smsfiltering.js
  ```

### 7. Output:

- The execution will generate an ARFF (Attribute-Relation File Format) file, typically used with WEKA machine learning software.

## Part 2: Using WEKA for SMS Spam Detection

### Step 1: Open WEKA

1. **Install WEKA** if not already installed. Download it from [WEKA official website](https://www.cs.waikato.ac.nz/ml/weka/).
2. **Launch WEKA** by running the WEKA application.

### Step 2: Load the ARFF File

3. Click on the **"Explorer"** button in the WEKA GUI.
4. Click **"Open file"** and navigate to your ARFF file containing the SMS spam dataset.

### Step 3: Select Class Attribute

5. Select the attribute representing the class label (e.g., "class" with values "spam" and "ham").

### Step 4: Choose Classifiers

6. Go to the **"Classify"** tab.
7. Choose the following classifiers one by one:
   - **J48** (Decision Tree)
   - **NaiveBayesMultinomial** (Multinomial Naive Bayes)
   - **IBk** (K-Nearest Neighbors)
   - **LibSVM** (Support Vector Machine)
   - **RandomForest** (Random Forest)

### Step 5: Set Cross Validation

8. WEKA uses **10-fold Cross Validation** by default. Leave it as is.

### Step 6: Run Classifiers

9. For each classifier, click **"Start"** to run it on the dataset.

### Step 7: Analyze Results

10. WEKA will display the results, including Accuracy, True Positive Rate (TPR), and False Positive Rate (FPR) for each classifier.

### Step 8: Compare Classifier Performance

11. Repeat Step 6 for each of the five classifiers to compare their performance in identifying SMS spam messages.
