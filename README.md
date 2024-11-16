# EIBFISR: Emotional Intensity-Based Feature and Insight Speech Ranker

EIBFISR is a Python-based open-source tool designed by Rees to analyze and rank speeches. It evaluates emotional intensity and effectiveness across specific traits such as **confidence**, **empathy**, **enthusiasm**, and **authority**. Using keyword-based analysis, it processes speech text to provide a quantitative assessment of emotional delivery, aiding in public speaking evaluations or speech improvement.

---

## Key Features

### 1. Emotional Trait Scoring
The script assigns scores to various emotional traits based on keywords found in the speech:
- **Confidence:** Words like "believe", "strong", or "assertive".
- **Empathy:** Words like "care", "understand", or "support".
- **Enthusiasm:** Words like "excited", "passionate", or "energy".
- **Authority:** Words like "command", "leader", or "expert".

### 2. Dynamic Trait Weight Adjustment
The script adjusts the importance of each trait based on the frequency and context of the related keywords. For example:
- If a speech contains many empathy-related keywords, the **Empathy** score will be higher.

### 3. Extensibility
- Easily extendable to add new emotional traits or adjust scoring systems.
- New keywords can be added to the configuration file, and scoring logic can be modified to suit different applications.

---

## Project Structure

### Files
- **`main.py`**: The core script that processes speech text, analyzes emotional traits, and generates rankings.
- **`README.md`**: Documentation that explains how to use the Speech Ranker, configure emotional traits, and run the script.
- **`requirements.txt`**: Lists the external Python dependencies (such as `nltk`, `re`, etc.) needed to run the Speech Ranker.

---

## How It Works

### 1. Keyword Matching
- The script tokenizes the speech text and searches for predefined keywords associated with specific emotional traits. For example:
  - Words like "I believe", "trust", and "strong" will trigger higher confidence scores.
  - Words like "listen", "care", or "understand" will increase empathy scores.

### 2. Adjusting Trait Weights
- After detecting the keywords, the script calculates the weight or score for each emotional trait.
- If a speech frequently uses keywords related to empathy, the empathy score will rise, while a lack of relevant keywords will result in a lower score for that trait.

### 3. Rank Generation
- The script generates a ranking for each emotional trait, providing insights into how effectively the speaker conveys each emotion.
  
---

## Customization

EIBFISR is flexible and can be adapted for different contexts:
- You can update the **`main.py`** file to fine-tune trait-to-keyword mappings.
- Adjust trait importance or add new emotional traits for analysis.

---

## Installation and Setup

### Prerequisites
- Python 3.7 or higher

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/ReesTheBeast/EIBFISR.git
   cd EIBFISR
Install the required dependencies:
bash
Copy code
pip install -r requirements.txt
Running the Tool
Provide the speech text in a .txt file.
Execute the script:
bash
Copy code
python main.py --input speech.txt
View the output:
Emotional trait scores
Rankings for each emotional trait
Use Cases
1. Public Speaking Evaluation
Evaluate speeches from competitions, debates, or presentations to assess emotional effectiveness.
2. Speech Coaching
Identify areas of strength and weakness in emotional delivery (e.g., improving empathy or confidence).
3. Sentiment Analysis
Analyze the emotional tone of political speeches, corporate presentations, or motivational talks.
4. AI/Chatbot Development
Integrate the Speech Ranker into chatbots or virtual assistants to enhance emotional cue recognition.
Example Output
Here is a sample ranking for a speech:

Emotional Trait	Score	Ranking
Confidence	85	1
Empathy	78	2
Authority	72	3
Enthusiasm	65	4
Contributing
Contributions are welcome! Feel free to submit issues or pull requests to improve the functionality.

Fork the repository.
Create a new branch for your feature:
bash
Copy code
git checkout -b feature-name
Commit and push your changes:
bash
Copy code
git commit -m "Add feature description"
git push origin feature-name
Submit a pull request.
License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgments
Designed and developed by Rees. Inspired by the need for data-driven emotional analysis in public speaking.

Contact
For questions or support, please contact:

Email: reesschofield@icloud.com

![image](https://github.com/user-attachments/assets/d56c03fe-33e0-430b-84f8-c5bed08ee250)
