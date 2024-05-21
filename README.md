# Currency Converter💵 ➡️ 💴
This project is a Currency Converter built using HTML, CSS, and JavaScript. It allows users to convert the currency of one country to another by utilizing an external API.

## Project Demo

Check out the live demo of the Currency Converter: [click here](https://siniekoo19.github.io/Currency-Converter/)

## Features
- Convert currency values between different countries.
- Fetch real-time exchange rates using an API.
- Simple and user-friendly interface.

## API Reference
```
https://cdn.jsdelivr.net/npm/@fawazahmed0/currency-api@latest/v1/currencies/{fromcountry}.json
```

## Fetching Exchange Rates
To fetch the exchange rates, the following code is used:

```bash
const BASE_URL = "https://cdn.jsdelivr.net/npm/@fawazahmed0/currency-api@latest/v1/currencies";
const url = `${BASE_URL}/${fromCurr.value.toLowerCase()}.json`;

let response = await fetch(url);
if (!response.ok) {
    throw new Error('Network response was not ok');
}

let data = await response.json();
const exchangeRate = data[fromCurr.value.toLowerCase()][toCurr.value.toLowerCase()];

```
## 🚀 About Me
👋 Hi there! I'm Sinchana Chatterjee, an enthusiastic and determined B.Tech student with a fervent aspiration to excel as a Web Developer.

## Authors
[@siniekoo19](https://github.com/siniekoo19)

## Acknowledgments
- Thanks to [githubs pages](https://siniekoo19.github.io/Simon-Says-Game/) for providing a platform to deploy my website.
- Thanks to the open-source community for their invaluable contributions to the tools and libraries used in this project.

## Feedback
If you have any feedback, please reach out to me at csinchana19@gmail.com
