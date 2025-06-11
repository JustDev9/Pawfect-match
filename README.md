# Pawfect Match

![Pawfect Match Logo](/public/Designer.png)

A comprehensive pet adoption platform designed to connect loving homes with pets in need. The system features a user-friendly interface for potential adopters and a robust admin panel for shelter staff to manage pets, adoption applications, and more.

## Features

### For Users:
- **Browse Pet Profiles**: Search and filter available pets based on species, age, temperament, etc.
- **Adoption Application**: Submit applications to adopt your perfect match
- **User Profiles**: Manage your personal information and track application status
- **Resources**: Access training tips and pet care information
- **Donations**: Support the shelter with financial contributions

### For Admins:
- **Dashboard**: View analytics and key metrics
- **Pet Management**: Add, edit, and track detailed pet information
- **Application Processing**: Review and process adoption applications
- **Pet History**: Track the history and adoption journey of each pet

## Technology Stack

### Frontend:
- **Vue.js 3**: JavaScript framework for building the user interface
- **Vite**: Next-generation frontend tooling
- **Vue Router**: For application routing
- **Pinia**: State management
- **Chart.js**: For analytics visualizations
- **Supabase Client**: For database interactions

### Backend:
- **Flask**: Python web framework
- **Supabase**: PostgreSQL database with built-in authentication
- **Mailjet**: For email notifications
- **JWT**: For secure authentication

## Project Structure

```
/
├── src/                  # Frontend source code
│   ├── assets/           # Static assets
│   ├── components/       # Reusable Vue components
│   ├── views/            # Vue pages
│   │   └── admin/        # Admin panel views
│   ├── config/           # Configuration files
│   ├── router/           # Vue Router configuration
│   ├── stores/           # Pinia stores
│   └── utils/            # Utility functions
├── backend/              # Flask backend
│   ├── app.py            # Main Flask application
│   └── requirements.txt  # Python dependencies
├── public/               # Public static assets
│   └── Img/              # Pet images
└── migrations/           # Database migration files
```

## Getting Started

### Prerequisites
- Node.js (v14+)
- npm or yarn
- Python (v3.8+)
- Supabase account

### Frontend Setup

1. Install dependencies:
```sh
npm install
```

2. Run development server:
```sh
npm run dev
```

3. Build for production:
```sh
npm run build
```

### Backend Setup

1. Navigate to the backend directory:
```sh
cd backend
```

2. Install Python dependencies:
```sh
pip install -r requirements.txt
```

3. Create a `.env` file with your environment variables:
```
SUPABASE_URL=your_supabase_url
SUPABASE_KEY=your_supabase_service_key
ADMIN_KEY=your_supabase_anon_key
FRONTEND_URL=your_frontend_url
```

4. Run the Flask application:
```sh
python app.py
```

## Deployment

The application is configured for deployment on Render with the following files:
- `render.yaml`: Configuration for Render deployment
- `frontend-render.yaml`: Frontend-specific configuration
- `render-build.sh`: Build script for Render

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgements

- [Vue.js](https://vuejs.org/)
- [Flask](https://flask.palletsprojects.com/)
- [Supabase](https://supabase.io/)
- [Render](https://render.com/)
