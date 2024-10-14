# Story Generator with Vocabulary Builder
#### Video Demo:  <URL HERE>
#### Description:

The **Story Generator with Vocabulary Builder** is an innovative application designed to help English learners improve their language skills through engaging storytelling. The project utilizes a generative AI model to create short stories that incorporate everyday vocabulary, making the learning process both enjoyable and effective. This application is perfect for intermediate to advanced English learners who want to enhance their language proficiency in a practical way.

## Project Overview

The primary goal of this project is to generate personalized stories that not only entertain but also educate. Each story is tailored to specific attributes, including meeting places, seasons, genres, tones, and English proficiency levels. This allows learners to experience a diverse range of narratives that are relevant to their everyday lives. The stories also include a vocabulary section, which explains key terms and provides practical usage examples.

### File Structure

- **main.py**: This is the main script of the application. It orchestrates the entire process, from generating the request text to saving the generated story and vocabulary to a CSV file. The main function calls various other functions to handle different tasks.

- **generate_request_text()**: This function generates a random request for the AI to create a story. It selects various attributes such as place, season, genre, and tone, and constructs a request string that guides the AI in producing relevant content.

- **gemini_works(request_text)**: This function interfaces with the generative AI model to create content based on the request text. It returns the generated story and vocabulary sections.

- **splitter(response_text)**: This function processes the AI's response, separating the story from the vocabulary section for easier access and understanding.

- **confirmation_prompt(story, vocabulary)**: This function prompts the user to confirm whether they want to share the generated story on Twitter. It provides a clear view of the content before proceeding.

- **split_and_save_tweets(story, filename, max_length)**: This function splits the story into tweet-sized segments and saves them to a specified file, allowing for easy sharing on social media.

- **vocabulary_handler(vocabulary, filename, max_length)**: Similar to the tweet splitter, this function processes the vocabulary section and saves it to the same file.

- **twitConnection()**: This function establishes a connection to the Twitter API, enabling the application to post the generated content directly to a user's Twitter account.

- **save_to_csv(request_text, story, vocabulary, english_level, filename)**: This function logs the generated content into a CSV file for future reference and analysis, maintaining a record of the stories generated and the vocabulary used.

## Design Choices

During the development of this project, several design choices were made to enhance usability and functionality:

1. **Generative AI Integration**: Leveraging a generative AI model allows for dynamic content creation, making each story unique and engaging.

2. **User Engagement**: By allowing users to customize the attributes of the stories, the application promotes a sense of ownership over the learning experience.

3. **Vocabulary Learning**: The inclusion of a vocabulary section helps reinforce language acquisition by providing definitions and usage examples, making it easier for learners to grasp new terms.

4. **Social Media Sharing**: Integrating Twitter functionality enables users to share their stories and vocabulary with a broader audience, encouraging community engagement and interaction.

## Future Enhancements

In future iterations of this project, additional features could be implemented to further enhance user experience. This may include:
- A more advanced user interface for easier navigation and interaction.
- Instagram and mobile application 
- Twitter seen, like data analysis regarding English level, concept
- Support for multiple languages to cater to a wider audience.
- Enhanced AI capabilities to generate stories more specific more realistic stories.
- Frequently sharing words to improve memorize words.

By combining language learning with creative storytelling, the **Story Generator with Vocabulary Builder** serves as a valuable tool for English learners seeking to improve their language skills in a fun and engaging way.
