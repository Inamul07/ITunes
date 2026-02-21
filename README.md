# iTunes Album Search

A responsive web application that allows users to search for music albums using the iTunes Search API. Users can search by artist name and view album details including artwork, title, price, and direct purchase links to the iTunes store.

## 🌟 Features

- **Real-time Search**: Search for albums by artist name using the iTunes API
- **Responsive Design**: Mobile-friendly interface built with Bootstrap
- **Album Information**: Display album artwork, title, and pricing
- **Direct Purchase Links**: Quick access to buy albums on iTunes
- **Clean UI**: Modern interface with custom styling and Google Fonts
- **No Results Handling**: User-friendly messaging when no matches are found

## 🚀 Demo

[Live Demo](https://inamul07.github.io/ITunes/)

## 📸 Screenshots

_Add screenshots of your application here_

## 🛠️ Technologies Used

- **HTML5**: Semantic markup structure
- **CSS3**: Custom styling with modern design patterns
- **JavaScript (ES5)**: Vanilla JavaScript for API calls and DOM manipulation
- **Bootstrap 4**: Responsive grid system and base styling
- **iTunes Search API**: Backend data source for album information
- **Google Fonts**: Roboto and Pacifico font families

## 📁 Project Structure

```
ITunes/
│
├── index.html          # Main HTML file
├── README.md           # Project documentation
│
├── css/
│   └── style.css       # Custom styles and layout
│
└── js/
    └── main.js         # Application logic and API integration
```

## 🔧 Installation

1. **Clone the repository**

    ```bash
    git clone https://github.com/yourusername/ITunes.git
    ```

2. **Navigate to the project directory**

    ```bash
    cd ITunes
    ```

3. **Open in browser**
    ```bash
    open index.html
    ```
    Or simply double-click the `index.html` file to open it in your default browser.

> **Note**: This is a static web application with no build process or dependencies required.

## 💡 Usage

1. Open the application in your web browser
2. Type an artist name in the search box (e.g., "The Beatles", "Taylor Swift")
3. Press Enter or submit the form
4. Browse through the album results displayed in a responsive grid
5. Click "Buy Now" on any album to visit its iTunes store page

### Search Tips

- Use full or partial artist names
- Search is case-insensitive
- Results are limited to albums only (not individual songs)

## 🔌 API Integration

This project uses the [iTunes Search API](https://developer.apple.com/library/archive/documentation/AudioVideo/Conceptual/iTuneSearchAPI/index.html):

**Endpoint**: `https://itunes.apple.com/search`

**Parameters**:

- `term`: Artist name (user input)
- `entity`: album (filters results to albums only)

**Example Request**:

```
https://itunes.apple.com/search?term=Adele&entity=album
```

## 🎨 Customization

### Styling

Modify [css/style.css](css/style.css) to customize:

- Color scheme (currently uses Material Design colors)
- Typography and font sizes
- Album card layout and spacing
- Responsive breakpoints

### Functionality

Edit [js/main.js](js/main.js) to:

- Change the number of results displayed
- Add filtering or sorting options
- Modify the data displayed for each album
- Implement additional API parameters

## 🌐 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Opera (latest)

## 📝 Code Highlights

### Object-Oriented JavaScript Pattern

The application uses a constructor function pattern for organization:

```javascript
var itunes = new itunes;
function itunes(){
    this.init = function(){ ... }
    this.search = function(){ ... }
    this.getData = function(artist){ ... }
    this.showArtist = function(obj){ ... }
}
```

### XMLHttpRequest for API Calls

Uses native browser API for HTTP requests (pre-Fetch API):

```javascript
var http = new XMLHttpRequest();
http.open("GET", url);
http.onreadystatechange = function(){ ... }
http.send();
```

## 🚧 Future Enhancements

- [ ] Add loading spinner during API requests
- [ ] Implement pagination for large result sets
- [ ] Add filter options (price range, release year)
- [ ] Include song previews with audio player
- [ ] Add search history/favorites functionality
- [ ] Refactor to use modern Fetch API or Axios
- [ ] Add error handling for network failures
- [ ] Implement debouncing for search input
- [ ] Add dark mode toggle
- [ ] Include unit tests

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 👤 Author

**Inamul Hassan**

- GitHub: [@inamul07](https://github.com/inamul07)
- Demo: [https://inamul07.github.io/ITunes/](https://inamul07.github.io/ITunes/)

## 🙏 Acknowledgments

- [iTunes Search API](https://developer.apple.com/library/archive/documentation/AudioVideo/Conceptual/iTuneSearchAPI/index.html) by Apple
- [Bootstrap](https://getbootstrap.com/) for the responsive framework
- [Google Fonts](https://fonts.google.com/) for typography
- Icons and inspiration from the iTunes ecosystem

---

**Note**: This is an educational project demonstrating API integration and vanilla JavaScript. It is not affiliated with or endorsed by Apple Inc.
