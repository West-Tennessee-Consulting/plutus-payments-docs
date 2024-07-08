# Plutus Payments Docs

This repository, `plutus-payments-docs`, is a collection of markdown files and images used for the documentation of the [West Tennessee Consulting website](https://github.com/West-Tennessee-Consulting/website). The documentation is published at [West Tennessee Consulting Docs](https://westtn.consulting/plutus-payments/docs/index/).

## Repository Structure

- **Markdown Files:** These files are the primary content of the documentation.
- **Images:** Stored in the `img` folder, these images are referenced within the markdown files.

## Build Process

The [website repository](https://github.com/West-Tennessee-Consulting/website) uses GitHub Actions for its build process. This process:

1. Pulls the documentation from this repository.
2. Converts the markdown files to HTML.
3. Publishes the HTML on the website.

### Key Details

- **Markdown to HTML Conversion:** The build process handles the conversion of markdown files to HTML.
- **Image Handling:** Images from the `img` folder in this repository are copied to the public folder of the Next.js website under `plutus/<contents of the img folder>`. The build process automatically adjusts the image links using a shell script. Refer to the script in the [deploy.yml](https://github.com/West-Tennessee-Consulting/website/blob/main/.github/workflows/deploy.yml#L40).

## Adding New Documentation

To add new documentation:

1. **Create Markdown Files:**
   
   - Add your new markdown files to the repository.
   - Ensure that any images used are placed in the `img` folder and referenced correctly.

3. **Update `index.md`:**
   
   - This file acts as the navigation bar on the left side of the documentation website.
   - You can add direct links or nested menus for your new markdown files.

### Example

- **Nested Menu:**
  
  ```markdown
  ## Customization
  [**View More About Customization**](/plutus-payments/docs/customization)
  ```

- **Direct Link:**
  
  ```markdown
  ## [**Direct Link**](/plutus-payments/docs/setup)
  ```

## Contribution Guidelines

1. **Fork the Repository:** Create your branch from `main`.
2. **Commit Your Changes:** Make sure your commit messages are descriptive.
3. **Create a Pull Request:** Ensure your PR describes the changes made and references any relevant issues.

## Links

- **Website Repository:** [West Tennessee Consulting Website](https://github.com/West-Tennessee-Consulting/website)
- **Documentation Site:** [Plutus Payments Docs](https://westtn.consulting/plutus-payments/docs/index/)

For any questions or issues, please open an issue in this repository or contact the repository maintainers.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

