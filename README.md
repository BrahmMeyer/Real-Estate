# Rod2Reel Business Delivery System

### 🌐 Setting up your Custom Domain
1. **Namecheap:** Go to your Advanced DNS settings.
2. **Add New Record:** - Type: `CNAME Record`
   - Host: `delivery` (this makes it delivery.yourdomain.com)
   - Value: `[your-github-username].github.io.` (Must end with a dot)
   - TTL: `Automatic`
3. **GitHub:** Go to your Repository Settings > Pages. 
   - Under "Custom Domain", type `delivery.yourdomain.com`.
   - Check "Enforce HTTPS".

### 🔗 URL Structure
- **Client Link:** `delivery.yourdomain.com/reel.html?id=RECORD_ID`
- **Dispatcher:** `delivery.yourdomain.com/send.html?id=RECORD_ID`
