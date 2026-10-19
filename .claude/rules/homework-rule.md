# Homework Rule

Course submission rules for DSCI 552. These are the TA's stated requirements; follow them
for every assignment in this repository.

## Required

1. **Submission channel.** All programming assignments are submitted through GitHub Classroom.
   TAs post an invitation link for each assignment before the due date. Clicking the link accepts
   the assignment and redirects to a private repository for it. Use **one** GitHub account for
   submission for the whole semester.

2. **Repository layout and paths.** Organize code and data files as the directory structure in the
   assignment figure, where the top-level folder is the root of the GitHub repository. Load data with
   **relative paths** so TAs can execute the notebooks without editing anything.
   - Never use `\` as a path separator, in absolute or relative paths — it is not recognized outside
     Windows. Always use `/`: `C:/Users/user1/Desktop`, `/usr/bin`, `../data/notebooks`.
   - Example of a correct path: `../data/vertebral_column_data/column_2C.dat`.
   - Never use an absolute path — TAs/CPs will likely fail to execute the code.
   - **Points are deducted** if TAs/CPs cannot execute the code because of an incorrect relative path.
   - `requirements.txt` is **mandatory** for every library installed. `README` and `.gitignore` are optional.

3. **Markdown cells.** Use markdown cells to indicate which question is being solved, and to report
   answers whenever the result cannot be explicitly output by code.

4. **Run all before submitting.** Use Jupyter's *Cell → Run All* to test that every cell works
   sequentially. Otherwise points may be lost to unseen exceptions when TAs execute the code.
   (Typical failure: a variable declared in an early cell is deleted later but still lives in the
   kernel's memory, so autocomplete keeps suggesting it and the notebook only breaks on a fresh run.)

5. **Local Jupyter only.** Finish the assignment in a local Jupyter Notebook. Do not develop in Google
   Colab and paste the code into a local `.ipynb` without testing — unexpected exceptions arise and
   TAs have to deduct points.

6. **Identification and file name.** Put **Name, GitHub Username and USC ID** in the **first cell** of
   the notebook. Name the file `Lastname_Firstname_HW(i).ipynb`, e.g. `Nandi_Soumyaroop_HW0.ipynb`.

## Additional suggestions (good practice, not rules)

1. **Group imports together**, preferably in the first cell. This documents all dependencies needed to
   run the notebook and avoids problems from cells running out of order during development.

2. **References and citations.** Keep a list of links/documents consulted while researching an algorithm
   in a markdown cell at the bottom of the notebook, to support the decisions and techniques used. It is
   also a useful personal collection for future reference.

3. **Plots and figures.** Label (and index) plots wherever possible to convey information quickly and
   concisely. Combining plots (e.g. matplotlib subplots) makes a submission drastically more presentable
   and builds data-visualization skill.

## Notes

- Once homework is uploaded, there is no need to follow up with TAs to confirm submission. GitHub records
  a timestamp; as long as it is within the deadline, it is submitted.
- **Always submit a copy of the `.ipynb` file in which every cell has been executed** (outputs saved).
