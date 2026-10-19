# GitHub Profile README Setup

## 1 Create the profile repository

Create a public GitHub repository with **exactly the same name as your GitHub username**. GitHub displays the repository README at the top of your profile.

For example, if the username is `Ankit-Jaipuriar`, the repository must be:

```text
Ankit-Jaipuriar/Ankit-Jaipuriar
```

## 2 Copy the files

Copy `README.md` to the root of that profile repository.

The contribution workflow is already included at:

```text
.github/workflows/contribution-snake.yml
```

## 3 Replace the GitHub username if needed

The profile README currently uses `Ankit-Jaipuriar` in its dynamic image URLs and project link. Replace that value everywhere if the actual GitHub username is different.

## 4 Run the animation workflow

Push the files, then open the **Actions** tab in the profile repository. Run **Generate contribution snake** manually once. The workflow publishes the animated SVG files to an `output` branch and refreshes them daily.

The workflow uses the `Platane/snk` action to generate SVGs from the profile contribution graph and then publishes those generated files. See the action repository documentation for its available visual options.
