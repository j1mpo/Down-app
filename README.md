# Down ☀️
### Personalized Activity Recommendation App

## About the Project

**Down** is a personalized activity recommendation web application designed to help users decide what to do based on their mood, available time, budget, energy level and personal preferences.

The main goal of Down is to make everyday decision-making easier by providing activity suggestions tailored to each user's current situation and needs.

## Features

- **Personalized Recommendations:** Recommends activities based on user preferences and contextual information.
- **Mood Selection:** Allows users to select their current mood.
- **Time & Budget Filters:** Considers the user's available time and budget.
- **Energy Level:** Adapts recommendations according to the user's energy level.
- **Weather Integration:** Retrieves real-time weather information using the Open-Meteo API.
- **Personalized Match Score:** Calculates how well each activity matches the user's preferences.
- **Activity Ranking:** Ranks activities according to their calculated recommendation scores.
- **Context Awareness:** Takes into account contextual factors such as time of day, day of the week and weather conditions.

## Recommendation System

Down implements a **rule-based personalized recommendation system**.

The system evaluates available activities using a scoring algorithm that considers multiple factors, including:

- User mood and preferences.
- Available time.
- Budget.
- Energy level.
- Weather conditions.
- Current contextual information.

Each activity receives a personalized score, allowing the application to rank suggestions and display the most relevant activities first.

This approach provides personalized recommendations without requiring a separately trained Machine Learning model.

## Technologies Used

- HTML5
- CSS3
- JavaScript
- Open-Meteo API

## How to Run

1. Clone or download this repository.
2. Open the project folder.
3. Open `index.html` in your browser.
4. Select your preferences and explore personalized activity recommendations.

An internet connection is required to retrieve real-time weather information.

## Project Purpose

Down aims to demonstrate how personalization, contextual data and recommendation algorithms can improve everyday decision-making.

By combining user preferences with real-time environmental information, the application helps users discover activities that better fit their current needs.

## Predictive Component

In addition to its recommendation system, Down incorporates a rule-based predictive component that estimates the potential success of an activity.

The prediction takes into consideration contextual factors such as:

- User preferences and mood.
- Available time and energy level.
- Budget compatibility.
- Current weather conditions.

Based on these factors, the application generates a **Predicted Success Score**, providing an indication of how suitable and likely to be successful an activity may be under the user's current circumstances.

This component complements the recommendation algorithm by adding a predictive perspective to the activity selection process.

*Note: The current implementation uses rule-based estimations rather than a trained Machine Learning model.*
