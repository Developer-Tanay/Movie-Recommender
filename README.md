# __Movie Recommender__

A simple API for movie recommendations.

## 🚀 Quick Start

### 1. Clone the Repository

```bash
git clone https://github.com/Developer-Tanay/Movie-Recommender.git
cd Movie-Recommender
```
**❗NOTE: Cloning may stuck because of Large Dataset size. Make sure You have a stable Internet connecion or try Downloading as a zip file then extract it to use.**

### 2. Set Up the Environment

Requirements are pinned for reproducibility.

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
```

### 3. Run the Application

```bash
uvicorn app:app --reload
```

- The API will be available at: `http://127.0.0.1:8000/recommend`

---

## 📦 API Endpoint

- **POST** `http://127.0.0.1:8000/recommend` — Send JSON Body

#### Example Request

```json
{
    "movie": "spiderman"
}
```

#### Example Response

```json
{
    "input_title": "spiderman",
    "matched_title": "Spider-Man",
    "recommendations": [
        {
            "movie_id": 559,
            "title": "Spider-Man 3",
            "score": 0.46757190011951816
        },
        {
            "movie_id": 558,
            "title": "Spider-Man 2",
            "score": 0.404079343830274
        },
        {
            "movie_id": 102382,
            "title": "The Amazing Spider-Man 2",
            "score": 0.2853908964926965
        },
        {
            "movie_id": 6488,
            "title": "Arachnophobia",
            "score": 0.24325212770525997
        },
        {
            "movie_id": 1930,
            "title": "The Amazing Spider-Man",
            "score": 0.2363058523195222
        }
    ]
}
```

---

## 🤝 Contributing

Contributions are welcome! Here’s how you can help:

1. **Fork** the repo
2. Create a new branch:

     ```bash
     git checkout -b feature/my-feature
     ```
3. Make your changes, add or update notebooks
4. Commit your work:

     ```bash
     git commit -m "Add feature: my feature"
     ```
5. Push your branch:

     ```bash
     git push origin feature/my-feature
     ```
6. Open a **Pull Request**—I’ll review and merge it!

---

## 📝 License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

**TL;DR**: clone ➕ install ➕ run ➕ explore ➕ update ➕ PR = ❤️

Happy modeling! 🚀
