# 📽️ BNI Slide Generator – Streamlit App

This is a web-based tool to:
- ✅ Create individual BNI presenter slides (with unique BNIP IDs, photo, logo, and member tags)
- ✅ Generate a full weekly presentation based on an Excel list and theme
- ✅ Download the final `.pptx` presentations with proper formatting

Built using **Streamlit**, **python-pptx**, and 100% open-source tools — no licenses or watermarks required.

---

## 📁 Folder Structure

```
bni-slide-generator/
├── main.py                      # The Streamlit app
├── requirements.txt             # Python dependencies
├── README.md                    # This file
├── bnipersons.csv               # BNIP ID tracker (auto-created if missing)
├── green_member_tag.png         # Tag image (Green Member)
├── gold_club_member_tag.png     # Tag image (Gold Club Member)
├── output/                      # Generated PPTX files
└── slides/
    ├── individual_template.pptx # Template for individual member slides
    ├── theme_slide.pptx         # Slide for the weekly theme
    └── constant_slide.pptx      # Final slide (e.g. thank you or contact info)
```

---

## 🚀 Running Locally

### 1. Install Dependencies
Make sure you have Python 3.8+ installed. Then install packages:
```bash
pip install -r requirements.txt
```

### 2. Run the Streamlit App
```bash
streamlit run main.py
```

---

## 🌐 Deploy on Streamlit Cloud (Free)

You can host this as a web app without setting up a server.

### Steps:
1. Push this folder to your GitHub repository
2. Visit [https://streamlit.io/cloud](https://streamlit.io/cloud)
3. Click **"New App"**, select your repo, and deploy
4. Share your public link with others!

> Note: Keep your `slides/` folder and `.png` files in the repo so the app runs as expected.

---

## 💡 Features

- Auto-generates unique BNIP IDs and saves them in `bnipersons.csv`
- Accepts photo and logo uploads per presenter
- Supports “Green Member” and “Gold Club Member” badges
- Replaces `NEXT_PRESENTER` dynamically in slides
- Adds a theme slide at the beginning and a constant slide at the end
- Exports downloadable `.pptx` files instantly

---

## ✅ Excel File Format

To generate a full presentation, upload an Excel file with at least one column:

| Name          |
|---------------|
| John Doe      |
| Jane Smith    |
| Alice Johnson |

---

## 📬 Feedback or Contributions

Feel free to:
- Fork the project
- Submit pull requests
- Report issues
- Suggest new features!

---

Created with ❤️ by [Your Name or Team Name]