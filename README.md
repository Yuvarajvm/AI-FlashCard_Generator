# AI FlashCard Generator

![Build Status](https://img.shields.io/badge/build-passing-brightgreen)
![Version](https://img.shields.io/badge/version-1.0.0-blue)
![License](https://img.shields.io/badge/license-MIT-yellowgreen)

## Features

- Generate flashcards from various inputs
- Multi-language support
- User-friendly interface
- Customizable flashcard templates
- Integration with educational resources

## Multi-Language Support

- Supports English, Spanish, French, German, and more.
- Localization options for user interfaces and content generation.

## Quick Start Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/Yuvarajvm/AI-FlashCard_Generator.git
   cd AI-FlashCard_Generator
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the application:
   ```bash
   npm start
   ```

## Architecture

The application is structured in a modular fashion, utilizing MVC (Model-View-Controller) architecture to separate concerns effectively.

- **Model:** Data handling, including database interaction.
- **View:** User interface components built with React.
- **Controller:** Logic that connects the model with the view.

## Database Schema

The database schema includes:

- **Users**: Stores user information
- **Flashcards**: Contains the details of generated flashcards.
  
Example schema:
```
Users
- id
- name
- email
- created_at

Flashcards
- id
- user_id
- content
- created_at
```

## API Reference

- **GET /api/flashcards**: Retrieve all flashcards.
- **POST /api/flashcards**: Create a new flashcard.
- **DELETE /api/flashcards/:id**: Delete a flashcard by ID.

## Deployment Guides

### Docker
To deploy the application using Docker, follow these commands:

```bash
docker build -t ai-flashcard-generator .
docker run -p 3000:3000 ai-flashcard-generator
```

### Heroku
1. Create a new Heroku app.
2. Push your code to Heroku:
   ```bash
   git push heroku main
   ```

## Contributing Guidelines

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Add new features'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a pull request.
