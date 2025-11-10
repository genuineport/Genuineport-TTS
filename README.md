---

## 💻 Usage

1. **Frontend**: Hosted on GitHub Pages  
   Example URL: `https://<your-username>.github.io/genuineport-tts/`  

2. **Backend**: Node.js server required for AI TTS processing  
   - Should expose a `/api/speak` endpoint
   - Accepts POST request with JSON:
     ```json
     {
       "text": "Hello, Genuineport TTS!",
       "voice": "default",
       "emotion": "neutral"
     }
     ```
   - Returns `audio_base64` and `mime` for frontend playback

3. **Connect frontend to backend**:  
   - In `script.js`, set `BASE_URL` to your backend URL:
     ```js
     const BASE_URL = 'https://your-backend-url.com';
     ```

---

## 📂 Deployment

### Frontend
- Push files to GitHub repository
- Enable **GitHub Pages** under `Settings → Pages`
- Set branch: `main` and folder: `/ (root)`
- Your frontend is now live at:
