# Polyglot Notebook Project: Data Analysis with C# and SQL

This project demonstrates how to use **Polyglot Notebook** in **Visual Studio Code (VS Code)** to perform data analysis using **C#** and **SQL**. The goal is to filter, group, and aggregate data from a CSV file, and then save the results to a new CSV file. The project also includes a guide on how to open and run the notebook in VS Code.

---

## Table of Contents
1. [What is Polyglot Notebook?](#what-is-polyglot-notebook)
2. [How to Open and Run the Notebook](#how-to-open-and-run-the-notebook)
3. [Project Overview](#project-overview)
4. [Data Files](#data-files)
5. [Output](#output)
6. [Advice for Users](#advice-for-users)
7. [Links and Resources](#links-and-resources)

---

## What is Polyglot Notebook?

Polyglot Notebook (formerly known as .NET Interactive Notebooks) is a tool that allows you to create interactive notebooks using multiple programming languages, including **C#**, **SQL**, **F#**, and **PowerShell**. It is similar to Jupyter Notebooks but is designed for .NET developers.

Polyglot Notebooks are ideal for:
- Data analysis and exploration.
- Prototyping and testing code.
- Sharing reproducible workflows.
- Combining code, visualizations, and markdown in a single document.

---

## How to Open and Run the Notebook

### Prerequisites
1. **Install Visual Studio Code**: Download and install [VS Code](https://code.visualstudio.com/).
2. **Install Polyglot Notebook Extension**:
   - Open VS Code.
   - Go to the Extensions Marketplace (`Ctrl+Shift+X`).
   - Search for **"Polyglot Notebooks"** and install the extension.
3. **Install .NET SDK**: Ensure you have the .NET SDK installed. Download it from [here](https://dotnet.microsoft.com/download).

### Steps to Open and Run the Notebook
1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/nuhyurdev/Questionnaire-Assessment.git
   ```
2. Open the project folder in VS Code:
   ```bash
   code Questionnaire-Assessment
   ```
3. Open the notebook file:
   - If the notebook is in `.ipynb` format, open `app.ipynb`.
   - If the notebook is in `.dib` format, open `app.dib`.
4. Run the notebook:
   - Open the notebook file in VS Code.
   - Use the **"Run"** button in the notebook toolbar to execute each cell.
   - Alternatively, use `Shift+Enter` to run the selected cell.

---

## Project Overview

### What Does This Project Do?
This project performs the following tasks:
1. **Reads a CSV file** (`exhibitA-input.csv`) containing play records with the following columns:
   - `PLAY_ID`: Unique identifier for each play.
   - `SONG_ID`: Unique identifier for each song.
   - `CLIENT_ID`: Unique identifier for each client.
   - `PLAY_TS`: Timestamp of when the song was played.

2. **Filters the records** for a specific date (`10/08/2016`).

3. **Groups the filtered records** by `CLIENT_ID` and counts the number of distinct `SONG_ID` values for each client.

4. **Saves the results** to a new CSV file (`output.csv`).

### Why This Project?
- **Learn Polyglot Notebook**: This project is a great way to learn how to use Polyglot Notebook for data analysis.
- **Combine C# and SQL**: It demonstrates how to use both C# and SQL in a single notebook for data manipulation.
- **Reproducible Workflow**: The notebook provides a reproducible workflow for filtering, grouping, and saving data.

---

## Data Files

### Input Data: `exhibitA-input.csv`
This file contains the raw play records. Here is an example of the data:

| PLAY_ID                          | SONG_ID | CLIENT_ID | PLAY_TS              |
|----------------------------------|---------|-----------|----------------------|
| 44BB190BC2493964E053CF0A000AB546 | 6164    | 249       | 2016-10-08 09:16:34  |
| 44BB190BC24A3964E053CF0A000AB546 | 544     | 86        | 2016-10-08 13:54:52  |
| 44BB190BC24B3964E053CF0A000AB546 | 9648    | 589       | 2016-10-08 06:08:53  |
| 44BB190BC24C3964E053CF0A000AB546 | 7565    | 656       | 2016-10-08 17:30:41  |
| 44BB190BC24D3964E053CF0A000AB546 | 8995    | 348       | 2016-10-08 02:40:39  |

### Output Data: `output.csv`
This file contains the results of the analysis. Here is an example of the output:

| DISTINCT_PLAY_COUNT | CLIENT_COUNT |
|---------------------|--------------|
| 2                   | 2            |
| 4                   | 1            |

---

## Output

The notebook generates the following output:
1. **Filtered Records**: Displays the records filtered for the date `10/08/2016`.
2. **Grouped Results**: Displays the number of distinct songs played by each client.
3. **Final Results**: Displays the number of clients for each distinct song count.
4. **Saved CSV**: The final results are saved to `output.csv`.

---

## Advice for Users

1. **Explore the Data**:
   - Open the `exhibitA-input.csv` file to understand the structure of the data.
   - Modify the notebook to explore different dates or additional columns.

2. **Experiment with Code**:
   - Try changing the filtering logic (e.g., filter by a different date).
   - Add new aggregations or groupings to the analysis.

3. **Visualize the Data**:
   - Use libraries like `XPlot.Plotly` or `Microsoft.Data.Analysis` to create visualizations of the results.

4. **Share Your Work**:
   - Share the notebook with others by uploading it to GitHub or exporting it as a PDF.

---

## Links and Resources

- [Polyglot Notebook Documentation](https://github.com/dotnet/interactive)
- [Visual Studio Code](https://code.visualstudio.com/)
- [.NET SDK Download](https://dotnet.microsoft.com/download)
- [C# Programming Guide](https://learn.microsoft.com/en-us/dotnet/csharp/)
- [SQL Tutorial](https://www.w3schools.com/sql/)

---

## Feedback and Contributions

If you have any questions, feedback, or suggestions, feel free to open an issue or submit a pull request. Your contributions are welcome!

Happy coding! 🚀