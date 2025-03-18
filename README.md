# alu_regex-data-extraction-PrincipieCyupe
![Image](https://github.com/user-attachments/assets/8afe8159-a70f-42b8-ab54-704dad0b99d7)
Formative-2_Frontend_Web_Development
# 🔍 Regex Data Extraction Project

## 📖 Project Overview
This project demonstrates the use of **Regular Expressions (Regex)** in **JavaScript** to extract structured data from text. It specifically focuses on identifying and extracting:
- 📧 **Email addresses**
- 🔗 **URLs**
- 📞 **Phone numbers**
- 💳 **Credit card numbers**
- 🏷️ **HTML tags**

## 🚀 Technologies Used
- **JavaScript (ES6+)**
- **Regular Expressions (Regex)**
- **Node.js** (for execution and testing)

## 🔍 Regular Expressions Used
The project uses the following regex patterns for extraction:

| Data Type             | Regex Pattern |
|----------------------|----------------------------------|
| **Email Addresses**  | `/[a-zA-Z0-9.]+@[a-zA-Z]+\.(com|co\.uk)/g` |
| **URLs**            | `/https?:\/\/[a-zA-Z]+\.example\.[a-zA-Z]+(\/[a-zA-Z]+)?/g` |
| **Phone Numbers**    | `/\(?\d{3,}\)?(\s|\.|-)\d{3,}(-|.)\d{4,}/g` |
| **Credit Card Numbers** | `/\d{4,}(\s|-)\d{4,}(\s|-)\d{4,}(\s|-)\d{4,}/g` |
| **HTML Tags**        | `/<[^>]+>/g` |

## 🛠️ How It Works
The program scans through a dataset and identifies patterns matching these five data types using **Regex**.  

### **📜 Example Input**
```json
{
    "Email addresses": ["user@example.com", "firstname.lastname@company.co.uk"],
    "URLs": ["https://www.example.com", "http://subdomain.example.org/pageLinks"],
    "Phone Numbers": ["(123) 456-7890", "123-456-7890", "123.456.7890"],
    "Credit card numbers": ["1234 5678 9012 3456", "1234-5678-9012-3456"],
    "HTML tags": ["<p>", "<div class='example'>", "<img src='image.jpg' alt='description'>"]
}
📜 Expected Output
Matches for Email addresses:
[ 'user@example.com', 'firstname.lastname@company.co.uk' ]

Matches for URLs:
[ 'https://www.example.com', 'http://subdomain.example.org/pageLinks' ]

Matches for Phone Numbers:
[ '(123) 456-7890', '123-456-7890', '123.456.7890' ]

Matches for Credit Card Numbers:
[ '1234 5678 9012 3456', '1234-5678-9012-3456' ]

Matches for HTML Tags:
[ '<p>', '<div class="example">', '<img src="image.jpg" alt="description">' ]
```

🛠️ How to Run the Code
1️⃣ Clone the Repository
git clone https://github.com/PrincipieCyupe/alu_regex-data-extraction-PrincipieCyupe.git
cd alu_regex-data-extraction-PrincipieCyupe
📌 Project Structure
/alu_regex-data-extraction-{YourUsername}/
│── onboard.js          # JavaScript file with regex implementation
│── README.md           # Project documentation

