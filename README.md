# Portfolio Project with Symfony and PostgreSQL on Platform.sh

This repository contains the source code for my personal portfolio built with Symfony and PostgreSQL, hosted on Platform.sh.

## Overview

This portfolio showcases my projects, skills, and professional journey. Built using Symfony for the back-end and PostgreSQL as the database, it provides a robust and scalable solution for displaying my work.

### Features

- **Project Showcase:** Detailed pages for each project, including descriptions, images, and technologies used.
- **Resume:** A dynamic version of my resume, highlighting my skills, experience, and education.
- **Contact Form:** A simple contact form for potential employers or collaborators to reach out to me.

## Getting Started

To run this project locally or deploy it to Platform.sh, follow the steps below.

### Prerequisites

- PHP 7.4 or higher
- Composer
- PostgreSQL
- Platform.sh CLI (for deployment)

### Installation

1. Clone the repository to your local machine:

    ```bash
    git clone https://github.com/yourusername/portfolio-symfony.git
    cd portfolio-symfony
    ```

2. Install dependencies using Composer:

    ```bash
    composer install
    ```

3. Create a `.env.local` file from the `.env` file and update the DATABASE_URL to your local PostgreSQL database credentials.

4. Run database migrations:

    ```bash
    php bin/console doctrine:migrations:migrate
    ```

5. Start the Symfony server:

    ```bash
    symfony server:start
    ```

Your application should now be running at `http://localhost:8000`.

### Deploying to Platform.sh

1. If you haven't already, sign up for an account at [Platform.sh](https://platform.sh/).

2. Initialize the project with Platform.sh:

    ```bash
    platform project:create --title "Portfolio on Symfony" --region your_region
    ```

3. Set up your environment:

    ```bash
    platform environment:init
    ```

4. Add your Platform.sh project Git remote and push:

    ```bash
    platform project:set-remote YOUR_PROJECT_ID
    git push platform master
    ```

Your application should now be deployed to Platform.sh!

## Contributing

Contributions, issues, and feature requests are welcome! Feel free to check [issues page](https://github.com/yourusername/portfolio-symfony/issues).

## License

Distributed under the MIT License. See `LICENSE` for more information.

## Contact

Your Name - email@example.com

Project Link: [https://github.com/yourusername/portfolio-symfony](https://github.com/yourusername/portfolio-symfony)
