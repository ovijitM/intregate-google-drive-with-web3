# Decentralized Cloud Storage - Google Drive + Web3 Integration

A web application that combines Google Drive storage with Web3 wallet authentication, creating a decentralized approach to cloud file management. Users can connect their Web3 wallet and upload files to Google Drive through a secure, wallet-authenticated interface.

![Decentralized Storage](https://img.shields.io/badge/Web3-Storage-blue)
![Google Drive](https://img.shields.io/badge/Google-Drive-green)
![MetaMask](https://img.shields.io/badge/MetaMask-Compatible-orange)

## ✨ Features

- **Web3 Wallet Integration**: Connect with MetaMask and other Web3 wallets
- **Google Drive Storage**: Seamless integration with Google Drive API
- **Wallet-Specific Folders**: Automatically creates dedicated folders for each wallet address
- **Multi-File Upload**: Upload multiple files simultaneously
- **File Management**: List and manage uploaded files
- **Responsive Design**: Bootstrap-powered responsive interface
- **Secure Authentication**: Dual authentication via Web3 wallet and Google OAuth

## 🚀 Prerequisites

Before you begin, ensure you have the following:

- **Web Browser** with Web3 support (Chrome, Firefox, Edge)
- **MetaMask** or another Web3 wallet extension installed
- **Google Account** with Drive API access
- **Google Cloud Project** with Drive API enabled
- **Basic web server** (for local development)

## 📋 Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/ovijitM/intregate-google-drive-with-web3.git
cd intregate-google-drive-with-web3
```

### 2. Set Up Google Drive API

1. Go to the [Google Cloud Console](https://console.cloud.google.com/)
2. Create a new project or select an existing one
3. Enable the Google Drive API
4. Create credentials (OAuth 2.0 Client IDs)
5. Configure the authorized JavaScript origins

### 3. Configure API Keys

Edit the JavaScript file (`test js traile 1`) and replace the placeholder values:

```javascript
const API_KEY = 'YOUR_ACTUAL_GOOGLE_API_KEY';
const CLIENT_ID = 'YOUR_ACTUAL_GOOGLE_CLIENT_ID';
```

### 4. Deploy the Application

For local development:
```bash
# Using Python
python -m http.server 8000

# Using Node.js (if you have http-server installed)
npx http-server

# Or simply open index.html in your browser (may have CORS limitations)
```

For production, deploy to any web hosting service (GitHub Pages, Netlify, Vercel, etc.)

## 🎮 Usage

### Getting Started

1. **Open the Application**: Navigate to your deployed URL or local server
2. **Connect Wallet**: Click "Connect Wallet" and authorize your MetaMask or Web3 wallet
3. **Authenticate Google**: The app will prompt for Google Drive permissions
4. **Upload Files**: Select files using the file picker and click "Upload"

### File Management

- **Automatic Organization**: Files are automatically organized in wallet-specific folders
- **Folder Naming**: Folders are named `DecentralizedStorage_[WalletAddress]`
- **File Listing**: View all uploaded files in the console (can be extended to UI)
- **Multiple Uploads**: Select and upload multiple files at once

### Security Features

- **Wallet Verification**: Only connected wallet owners can access their files
- **Google OAuth**: Secure Google authentication for Drive access
- **Isolated Storage**: Each wallet gets its own dedicated folder

## 📁 Project Structure

```
├── index.html              # Main application interface
├── styles.css              # CSS styling and responsive design
├── test js traile 1        # Core JavaScript functionality
└── README.md              # Project documentation
```

### Key Components

- **`index.html`**: Bootstrap-based responsive UI with file upload form
- **`styles.css`**: Custom styling for wallet connection states and UI
- **`test js traile 1`**: Main application logic including:
  - Web3 wallet connection handling
  - Google Drive API integration
  - File upload and management functions
  - UI state management

## 🛠 Technologies Used

### Frontend
- **HTML5** - Structure and semantics
- **CSS3** - Styling and responsive design
- **Bootstrap 4.5.2** - UI framework and components
- **JavaScript (ES6+)** - Application logic

### APIs & Libraries
- **Web3.js** - Ethereum blockchain interaction
- **Google Drive API v3** - File storage and management
- **Google API JavaScript Client** - API authentication and requests

### Web3 Integration
- **MetaMask** - Primary wallet provider
- **Ethereum** - Blockchain network support
- **Web3 Provider** - Wallet connectivity

## ⚙️ Configuration Options

### Google Drive API Settings
```javascript
const SCOPES = 'https://www.googleapis.com/auth/drive.file';
```

### Wallet Connection
- Supports MetaMask and Web3-compatible wallets
- Automatic wallet state persistence in localStorage
- Graceful fallback for non-Web3 browsers

### File Upload Settings
- Multiple file support
- Empty file validation
- Error handling for upload failures

## 🔧 Development

### Local Development

1. Clone the repository
2. Configure Google API credentials
3. Run a local web server
4. Test with MetaMask in development mode

### Adding Features

The codebase is structured to easily add:
- Additional storage providers
- Enhanced file management UI
- File sharing capabilities
- Encryption features
- IPFS integration

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## ⚠️ Security Considerations

- **API Keys**: Never commit actual API keys to version control
- **Wallet Security**: Always verify wallet connections
- **HTTPS**: Use HTTPS in production for secure wallet connections
- **CORS**: Configure proper CORS settings for production deployment

## 🐛 Known Issues

- JavaScript file naming (`test js traile 1`) should be standardized
- Missing `app.js` file referenced in HTML
- Console-only file listing (could be enhanced with UI)

## 📞 Support

If you encounter any issues or have questions:
- Open an issue on GitHub
- Check the browser console for error messages
- Ensure MetaMask is properly installed and connected
- Verify Google API credentials are correctly configured

---

**Built with ❤️ for the decentralized web**