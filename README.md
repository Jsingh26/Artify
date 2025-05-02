# Artify - Art Auction Platform

![Artify Logo](images/artifylogo.svg)

## Overview

Artify is a modern online auction platform designed specifically for art enthusiasts. The platform allows artists to showcase and sell their artwork while providing art collectors with a user-friendly interface to discover and bid on unique pieces. With a focus on paintings, sculptures, and crafts, Artify brings the traditional art auction experience to the digital world.

## Features

- **User Authentication**: Secure login and registration system
- **Art Listing**: Artists can list their artwork with descriptions, images, and starting prices
- **Auction System**: Real-time bidding functionality with set end times
- **Categories**: Browse artwork by categories including paintings, sculptures, and crafts
- **Responsive Design**: Optimized viewing experience across various devices

## Tech Stack

- **Frontend**: HTML, CSS, JavaScript
- **Backend**: PHP
- **Database**: MySQL
- **Session Management**: PHP Sessions

## Database Structure

The application uses a MySQL database with the following tables:

- **users**: Stores user account information
- **items**: Contains artwork details including images and auction parameters
- **bids**: Records all bids placed on auction items

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/artify.git
   ```

2. Set up a local web server with PHP support (like XAMPP, WAMP, or MAMP)

3. Import the database structure:
   ```
   mysql -u username -p database_name < database.sql
   ```

4. Configure the database connection:
   - Create a `config.php` file in the `php` directory with your database credentials:
   ```php
   <?php
   $host = 'localhost';
   $dbname = 'artify';
   $username = 'your_username';
   $password = 'your_password';

   try {
       $pdo = new PDO("mysql:host=$host;dbname=$dbname", $username, $password);
       $pdo->setAttribute(PDO::ATTR_ERRMODE, PDO::ERRMODE_EXCEPTION);
   } catch (PDOException $e) {
       die("Connection failed: " . $e->getMessage());
   }
   ?>
   ```

5. Create an `images` directory in the root folder and ensure it has write permissions for image uploads

6. Access the application through your local web server

## Usage

### For Artists

1. Create an account or log in
2. Click on "Add to Auction" on the home page
3. Fill out the artwork details including title, description, image, starting price, and auction end time
4. Submit the form to list your artwork

### For Collectors

1. Create an account or log in
2. Browse available artwork by category or view all current auctions
3. Click on an artwork to view details and bidding history
4. Place a bid higher than the current highest bid
5. Receive notifications when you're outbid or when you win an auction

## Directory Structure

```
artify/
├── css/
│   └── style.css
├── images/
│   ├── artifylogo.svg
│   └── [artwork images]
├── js/
│   └── script.js
├── php/
│   ├── add_item.php
│   ├── config.php
│   ├── login.php
│   └── register.php
├── add_item.php
├── auction.php
├── debug_auction.php
├── index.php
├── login-registration.php
└── database.sql
```

## Screenshots

registratio-page:

![WhatsApp Image 2025-05-02 at 20 36 23_8a44f52f](https://github.com/user-attachments/assets/2f77b27d-f358-44bb-867b-bed0ebba4749)

login-page:

![WhatsApp Image 2025-05-02 at 20 37 06_d18ee5e0](https://github.com/user-attachments/assets/d039aea5-6bd9-42f2-86c5-858b839e3ca2)

index/dashboard-page:

![WhatsApp Image 2025-05-02 at 20 37 28_a8807000](https://github.com/user-attachments/assets/53ea8c6e-8308-4283-8a5a-2979b8fce7ee)
![WhatsApp Image 2025-05-02 at 20 37 49_221ac770](https://github.com/user-attachments/assets/5c151d4f-481f-4df5-9d3d-04a72d7748d1)
![WhatsApp Image 2025-05-02 at 20 38 07_d3392f80](https://github.com/user-attachments/assets/4d4f6eeb-7043-4582-8123-cdbd47dbde2d)

add-item-page:

![WhatsApp Image 2025-05-02 at 20 45 05_9cc9b78a](https://github.com/user-attachments/assets/7057f974-1e02-49ab-a199-5ed0ddbd4d52)

auction-page:

![WhatsApp Image 2025-05-02 at 20 46 18_59bbce59](https://github.com/user-attachments/assets/14c72a22-5f2b-4e90-bc9c-d1044d17f380)
![WhatsApp Image 2025-05-02 at 20 46 43_4604bd66](https://github.com/user-attachments/assets/28c1741a-1ce8-4c88-98fd-d41011775a34)
![WhatsApp Image 2025-05-02 at 20 47 08_9a3ecf1d](https://github.com/user-attachments/assets/1171b746-401c-4ce6-8523-ae6ce939901d)

updated-Bid:

![WhatsApp Image 2025-05-02 at 20 47 26_ffbd2e7b](https://github.com/user-attachments/assets/1093f541-0882-4ead-939e-0365bdfaac57)

MySQL-Database:

![WhatsApp Image 2025-05-02 at 20 50 00_81a70a4d](https://github.com/user-attachments/assets/c3f36420-8ffe-4861-b8f7-92eda05d66b9)


## Future Enhancements

- Implementing a search functionality
- Adding user profiles with ratings and reviews
- Integration with payment gateways
- Social media sharing capabilities
- Direct messaging between users
- Featured auctions on the homepage

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the Apache 2.0 License - see the LICENSE file for details.

## Contact

Japinder Singh - [japinder2004@gmail.com]
neal malik - [nealmalik07@gmail.com]

Project Link: [https://github.com/Jsingh26/artify](https://github.com/Jsingh26/artify)

## Acknowledgments

- [Font Awesome](https://fontawesome.com) for icons
- All the artists who inspired this project
