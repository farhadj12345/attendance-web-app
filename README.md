# Mobile Attendance Web-App

A web-based attendance management system with role-based access control and geolocation verification.

> **Note:**  
> The app is mobile-friendly and can be used on phones and tablets.  
> To use on a mobile device, serve the app from a local server and open the URL in your mobile browser on the same Wi-Fi network.

## Features

### Student Features
- Mark attendance as Present/Absent for assigned courses
- Location-based attendance verification
- View only assigned courses
- Password reset functionality
- Real-time attendance status updates

### Professor Features
- View attendance dashboard for assigned courses
- Monitor student attendance with timestamps and location data
- Track attendance records in real-time
- View students assigned to each course

### Admin Features
- Manage users (students, professors, admins)
- Manage courses
- Assign courses to students and professors
- View all attendance records
- Reset user passwords

## Allowed Locations
The system verifies attendance from these locations:
1. Ostim Technical University - Ostim, 100. Year Blvd. 55/F, 06374 Yenimahalle/Ankara (500m radius)
2. Coffee Lab Çankaya (100m radius)
3. Primary Home Location (100m radius)
4. Alternate Home Location (100m radius)

## Technical Implementation

### Authentication
- Role-based login system (Student/Professor/Admin)
- Session management using localStorage
- Password reset functionality
- Secure role verification

### Geolocation Features
- Real-time location verification
- Multiple allowed locations support
- Distance calculation from approved locations
- Location precision control
- Graceful geolocation error handling

### Storage
All data is stored in localStorage:
- `users`: User credentials and roles
- `courses`: Available courses
- `professorCourses`: Course assignments for professors
- `studentCourses`: Course assignments for students
- `attendance`: Attendance records with timestamps and location data

## Project Structure
```
├── index.html         # Main application interface
├── login.html         # Login page
├── admin.html         # Admin dashboard
├── courses.html       # Attendance marking interface
├── styles.css         # Shared styles
<!-- ...other files... -->
```

## Accessing the Web App on Mobile via GitHub Pages

You can easily access this attendance web app on your mobile device using GitHub Pages. Once the project is deployed to GitHub Pages, it is available as a public website. To open the app on your phone or tablet, simply navigate to the GitHub Pages URL in your mobile browser. The URL will typically be:

```
https://<your-github-username>.github.io/<repository-name>/
```

For example, if your GitHub username is `farhadj12345` and your repository is `attendance-web-app`, the URL would be:

```
https://farhadj12345.github.io/attendance-web-app/
```

Open this link in your mobile browser (such as Chrome or Safari). The app is designed to be mobile-friendly and will automatically adjust its layout for smaller screens. You do not need to install anything—just use your browser.

**Note:**  
- Make sure your repository is public and GitHub Pages is enabled in your repository settings.
- If you make changes to the app, it may take a few minutes for updates to appear on GitHub Pages.
- For full functionality (such as geolocation), you may need to allow location permissions in your mobile browser.

## Contributors

- Ahrafal Amal (@ahrafal-amal)

## License

MIT

&copy; 2025 Mobile Attendance Web-App
