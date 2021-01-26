# Wi5 Front-end Technical Test

## Getting started
Please fork this repository to get started.

### Requirements
Ensure you have these installed:
- Node LTS
- NPM or Yarn: [https://classic.yarnpkg.com/en/docs/install/](https://classic.yarnpkg.com/en/docs/install/)

## Build setup
We will give these commands using Yarn however this can be substituded for NPM.

``` bash
# install dependencies
$ yarn

# serve with hot reload at http://localhost:3000
$ yarn run dev
```

## Notes
- Use modern ES6 methods where appropriate
- We use BEM for our class names
- You only need to consider how the work renders on a desktop browser, not tablets or mobile
- We will look at your work in Chrome

## Test tasks
The test involves displaying a list of articles which are to be filterable and searchable.

1. Add a new route, accessible at `/articles`.

2. Create a reusable component inside that page's route template which displays a simple list of the articles.
 - The data for these articles should be imported from the 'articles' store module (`/store/articles`).
 - The list should show the article's title and date. Add a little basic styling to the list - but you won't be judged on the design.

3. Add a select (dropdown) form element at the top of the page. This should act as a category filter for the visible articles. Add options in the select element to filter by these categories:
 - All articles (default)
 - General category
 - News category
 - Case Studies category

 In the article store data you will see that the `categories` property contains the 'slugs' of the related categories. You should use this data to filter on.
 
4. Add a text input form element at the top of the page. This should act as a text search, which filters the list of articles based on their titles. Eg. if a user enters 'Wi5' in the search field, only articles containing the string 'Wi5' should display. Clearing the field should show the full list of articles again.

5. If you have time, make the category filter work in conjunction with the search field. Eg. if the 'News' category is selected and the user searches for 'Wi5', only display articles that belong to the 'News' category with 'Wi5' in its name.
