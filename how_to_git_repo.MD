# A General Structure of a GitHub Repository

## Root Directory
- `README.md`
  Provide an overview of the project and its contents.
## `/data`
- **`README.md`**  
  Explain the purpose of the data folder and provide details on the data.

### Guidelines:
- Do not include large files (>50MB). If you have large files:
  - Add them to your `.gitignore` file.
  - Mention them in the `README.md` and keep the actual files on a file server (e.g., reach out to Dr. Li) and on your computer.
- If data comes from external sources, state this in the `README.md`.
- Provide raw data and ensure all steps (e.g., parsing) are repeatable.

## `/code`
- **`README.md`**  
  Include details about the codebase and how to run it.
- **`requirements.txt`**  
  List the necessary dependencies for the project.
- Add subfolders as needed for organization.

## `/latex`
This directory is mapped to Overleaf. Note:
- The entire repository will sync to Overleaf, but only the `/latex` folder is relevant.
- Files/Folders:
  - `main.tex`
  - `references.bib`
  - `references` (folder for bibliographic PDFs)
  - `figures` (folder for LaTeX-specific figures)

## `/images`
Include project-related images and visualizations.

## `/references`
- Include all relevant PDFs following a consistent naming convention.

## `/slides`
- Files:
  - `slides.pptx` (for PowerPoint slides)
  - `slides.tex` (if using Beamer for LaTeX slides)
- Ensure slides are conference-ready (background, problem, methodology, etc.).

## Other Considerations
- Ensure the repository is a **standalone, one-stop** resource for a manageable "paper" or R&D topic.
- For larger projects:
  - Break them into smaller repositories.
  - Each repository should lead to a paper or specific topic.
- Not all repositories require this exact structure — be adaptive.

### General Workflow
- Always fetch the newest version before working on it
- Create your own branch and start to work on it
- Create a pull request to merge your branch to the main branch
- If you fork the original repo, fine. You can still make a pull request

### Code Best Practices
1. Remove unused dummy code from `.ipynb` or `.py` files.
2. Remove unused files.
3. Add proper markdown headings in `.ipynb` or `.py`.
4. Add comments to your code.
5. Refactor & optimize code after initial development. You can do the dirty trial-n-error in your branch! When you are done, commit the clean code to the main branch.

### Technical Notes (**Internal use only**)
- Ensure the code (repository) is on the GPU server's `shared_space`, if applicable.
- If you need help setting up GitHub in your folder on the GPU server, contact Dr. Li.

