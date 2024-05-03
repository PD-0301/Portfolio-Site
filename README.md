# Portfolio Site

This portfolio site serves as a showcase of your work, skills, and experiences. It provides a professional platform for you to display your projects and works, resume, and contact information. 
<br> 

This project is built using Jekyll, a simple, blog-aware static site generator.

## Features

- **Responsive Design**: The site is designed to be fully responsive, ensuring a seamless experience across devices of all sizes.
- **Jekyll Integration**: Built with Jekyll, making it easy to manage and update content using Markdown files.
- **Customizable**: The site's layout and styles are highly customizable, allowing you to tailor it to your preferences.
- **Project Showcase**: Includes a section to showcase your works with descriptions and links.
- **Resume Section**: Provides a section to display your resume or CV.

## Local Installation

To run the portfolio site locally, you'll need to have Jekyll installed. If you haven't already, you can install it by following the [official installation guide](https://jekyllrb.com/docs/installation/).

Once Jekyll is installed, follow these steps:

1. Fork this repository: Click the "Fork" button at the top-right corner of this page to create a copy of this repository in your GitHub account.
1. Clone your forked repository: Clone the forked repository to your local machine using the following command: `git clone https://github.com/your-username/portfolio-site.git`
2. Navigate to the project directory: `cd portfolio-site`
3. Install dependencies: `bundle install`
4. Start the Jekyll server: `bundle exec jekyll serve`
5. Open your browser and go to `http://localhost:4000` to view the site.

## Usage

After setting up the site locally, you can customize it to your liking:

- Modify the `_config.yml` file to update site settings such as title, description, `url`, `baseurl`, etc.
- Update Markdown files in the `_WORKS` directory to add or edit project descriptions.
- Customize the styles in the `assets/css/styles.css` to your liking.

## Hosting on GitHub Pages with Custom URL

GitHub Pages offers free hosting for static websites, including Jekyll-based sites like this portfolio project. You can easily deploy your site to GitHub Pages and even use a custom domain name for your site.

### Steps to Host on GitHub Pages:

1. **Prepare Your Repository**:
   - Make sure your Jekyll site is ready and properly configured.
   - Push your changes to `gh-pages` branch.

2. **Configure Your Repository**:
   - Go to your repository's settings page.
   - Scroll down to the "GitHub Pages" section.
   - Select the source branch for GitHub Pages as `gh-pages` & `/(root)` folder.
   - Optionally, configure a custom domain if you have one.

3. **Deploy Your Site**:
   - Once configured, GitHub Pages will automatically deploy your site.
   - You can access your site at `https://your-username.github.io/repository-name`.
   - If you've configured a custom domain, it may take some time for the changes to propagate.

### Using a Custom Domain:

If you have a custom domain name (e.g., `www.yourname.com`), you can set it up to point to your Portfolio site. You can also refer to the github's [official documnetaion](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/about-custom-domains-and-github-pages) to Configure your custom domain for your GitHub Pages site.

1. **Add a CNAME File**:
   - In your forked repository, create a file named `CNAME` (without any file extension).
   - Inside the `CNAME` file, add your custom domain name (e.g., `www.yourname.com`).

2. **Configure DNS Settings**:
   - Log in to your domain registrar's website and navigate to the DNS settings for your domain.
   - Add a CNAME record pointing to `your-username.github.io`.

3. **Update GitHub Pages Settings**:
   - In your repository's settings, add your custom domain name in the "Custom domain" field.
   - GitHub Pages will automatically update the DNS configuration to use your custom domain.

4. **Verify Configuration**:
   - It may take some time for DNS changes to propagate.
   - Once propagated, you should be able to access your site using your custom domain.

By following these steps, you can host your portfolio site on GitHub Pages and give it a professional touch with a custom domain name.

<br>

Feel free to explore and experiment with different configurations to make the site your own!

