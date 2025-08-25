# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-swc](https://github.com/vitejs/vite-plugin-swc/blob/main/packages/plugin-swc/README.md) uses [SWC](https://swc.rs/) for Fast Refresh

## Deployment

This app is configured for cloud deployment with a Procfile. The frontend will be built and served using the `serve` package.

### Environment Variables

For production deployment, you need to set the following environment variable:

- `VITE_API_URL`: The URL of your backend API (e.g., `https://your-api-domain.com`)

### Cloud Provider Setup

1. **Heroku**: Set the environment variable in your app settings
2. **Railway**: Add the environment variable in your project variables
3. **Render**: Set the environment variable in your service configuration

### Local Development

For local development, the app will use `http://localhost:8000` as the default API URL. You can override this by setting the environment variable:

```bash
export VITE_API_URL=http://localhost:8000
```

### API Endpoints

The app expects the following API endpoints:
- `GET /jobs` - List all jobs
- `GET /jobs/:id` - Get a specific job
- `POST /jobs` - Create a new job
- `PUT /jobs/:id` - Update a job
- `DELETE /jobs/:id` - Delete a job
