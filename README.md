Project name: Machine learning-based SMS Spam Filtering

Part 1: Below are the instructions to execute the code and generate an arff file.

1\. Please make sure the below files are in the same directory.

a. smsfiltering.js

b. english_big.txt

2\. Open the working directory where the files are located through command prompt or terminal.

3\. Please ensure you have Node.js installed on your machine, we need this to run our code while since it is written in JavaScript.

4\. If Node.js is installed, please proceed to step 6 directly to run the code. Else, please follow the instructions in step 5 to install Node.js on your machine.

5\. To run JavaScript code on Windows, Linux, or macOS machines, you'll need to use the Node.js runtime, which allows you to execute JavaScript code outside of web browsers. Here are the steps to run JavaScript code:

A. Install Node.js (if not already installed):

- Windows: You can download the Windows Installer for Node.js from the official Node.js website (https://nodejs.org/), run the installer, and follow the installation instructions.

- Linux: You can use your system's package manager to install Node.js.

For example, on Ubuntu or Debian, you can use \`apt\`:

> sudo apt update

> sudo apt install nodejs

On Red Hat, CentOS, or Fedora, you can use \`yum\` or \`dnf\`:

> sudo yum install nodejs

Be sure to install Node Package Manager (npm) as well.

- macOS: You can use Homebrew to install Node.js on macOS. If you don't have Homebrew installed, you can find installation instructions at https://brew.sh/. After installing Homebrew, run:

> brew install node

B. Run JavaScript Code:

- Using Command Line (Terminal): Open your command line terminal (Command Prompt on Windows, Terminal on macOS, or Terminal on Linux). Navigate to the directory where your JavaScript file is located. Use the \`node\` command to run your JavaScript file. For example:

> node .js

In our case, we use below file to execute our code -

> node smsfiltering.js

- Using an IDE: Many code editors and IDEs have built-in support for running JavaScript code. If you're using an IDE like Visual Studio Code, you can open your \`.js\` file and use its built-in terminal or integrated terminal to run your script. Just open the terminal and run \`node smsfiltering.js\`.

C. View Output:

The terminal or console will display the output of your JavaScript code. You can also use \`console.log()\` in your code to print messages and data to the terminal for debugging and testing purposes.

6\. Execute the below command -

> node smsfiltering.js

7\. It will generate an ARFF (Attribute-Relation File Format) file which is a plain text file format that is commonly used with the WEKA machine learning software.

Part 2 : How to Use WEKA for SMS Spam Detection

These instructions will guide you through the process of opening an ARFF file in WEKA and running binary classifiers to identify SMS spam messages. The following five classification algorithms with Cross Validation will be used: Decision Tree (J48), Multinomial Naive Bayes, K-Nearest Neighbors, SVM (LibSVM), and RandomForest. You will need to follow these steps to analyze the experimental results, including Accuracy, True Positive Rate (TPR), and False Positive Rate (FPR) for each classifier.

Step 1: Open WEKA

1\. Ensure you have WEKA installed on your system. If it's not already installed, you can download it from the WEKA website (https://www.cs.waikato.ac.nz/ml/weka/).

2\. Launch WEKA by running the WEKA application.

Step 2: Load the ARFF File

3\. In the WEKA GUI, click on the "Explorer" button to open the Explorer interface.

4\. In the Explorer, click on the "Open file" button to load your ARFF file. Navigate to the directory where your ARFF file is located and select it. The ARFF file should contain your SMS spam dataset and the associated features.

Step 3: Select the Class Attribute

5\. Once your dataset is loaded, select the attribute that represents the class label. In this case, it should be "class" with values "spam" and "ham." We will use this attribute for binary classification.

Step 4: Choose Classifiers

6\. Click on the "Classify" tab in WEKA's Explorer.

7\. Under the "Classifier" section, you will see a list of classifiers. Choose the following classifiers one by one:

- J48 (Decision Tree)

- NaiveBayesMultinomial (Multinomial Naive Bayes)

- IBk (K-Nearest Neighbors)

- LibSVM (Support Vector Machine)

- RandomForest (Random Forest)

Step 5: Set Cross Validation

8\. By default, WEKA performs Cross Validation with K=10. You can leave the Cross-Validation settings at their defaults.

Step 6: Run Classifiers

9\. For each classifier selected in Step 4, click the "Start" button to run the classifier on your dataset. WEKA will evaluate the classifier's performance using Cross Validation.

Step 7: Analyze Results

10\. Once the classification is complete, WEKA will display the results, including Accuracy, True Positive Rate (TPR), and False Positive Rate (FPR) for each classifier. Note the performance metrics for analysis.

Repeat Step 6 for each of the five classifiers to compare their performance in identifying SMS spam messages. The classifier with the best performance based on your analysis can be considered as the most suitable for your SMS spam detection task.
