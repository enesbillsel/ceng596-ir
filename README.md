
# Semantic Query Expansion via SBERT-Enhanced Pseudo-Relevance Feedback

Our project aims to improve PRF by using SBERT, a sentence embedding model that captures semantic relationships. We extract semantically similar sentences from BM25 top-ranked documents using SBERT. Then, we identify key phrases from these sentences and use them to expand the original query. This approach brings context-aware terms better aligned with user intent.

## How to Use

1. Download or clone this repository.

2. Open the notebook file (`IR_Project.ipynb`) on [Google Colab](https://colab.research.google.com/):

   - Go to [Google Colab](https://colab.research.google.com/).
   - Click **File > Upload notebook**.
   - Upload the downloaded `IR_Project.ipynb` file.

3. **Prepare the dataset:**

   - Download the dataset folder from [this link](https://drive.google.com/drive/folders/1YhAtURXgUp0QlldXcDn1bzgCiQK6GvI5).
   - Upload or sync this folder to your **Google Drive** (e.g., under `MyDrive/AssociatedPressDataset`).
   - The notebook expects the data to be available at the path:  
     `/content/drive/MyDrive/AssociatedPressDataset/`

4. Run all cells sequentially (Shift + Enter) to execute the project.

5. **Mounting Google Drive in Colab**

   When you run the notebook, you will see a prompt like this:

   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```

   Running this cell will ask you to authorize access:

   1. Click the link that appears in the output.
   2. Select your Google account.
   3. Copy the authorization code provided.
   4. Paste the code back into the Colab input box and press Enter.

   After this, your Google Drive will be mounted at `/content/drive` and accessible within the notebook.

## Notes

- Make sure to mount Google Drive when prompted to access the dataset.
- Ensure a stable internet connection for package installations and downloading models.
- The user interface can be launched by running its code block. It starts a free server where users can search test queries using different retrieval methods applied in the project.