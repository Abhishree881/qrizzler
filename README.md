# MVC Node.js Application with Prisma, GraphQL, and Express

## Overview

This is a Node.js application structured using the MVC (Model-View-Controller) pattern. It utilizes Prisma as an ORM for database interactions, GraphQL for API communication, and Express as the web framework.

## Features

- **MVC Architecture**: Organizes code into models, views, and controllers for better separation of concerns.
- **Prisma**: A powerful ORM that simplifies database access and management.
- **GraphQL**: Provides a flexible and efficient way to query and manipulate data.
- **Express**: A minimal and flexible Node.js web application framework.

## Getting Started

### Prerequisites

- Node.js (version 14 or higher)
- npm or yarn
- A PostgreSQL database (or any other supported database)

### Installation

1. Clone the repository:

   
   git clone https://github.com/yourusername/your-repo.git
   cd your-repo
   

2. Install dependencies:

   
   npm install
   

   or

   
   yarn install
   

3. Set up your database:

   - Create a `.env` file in the root directory and configure your database connection string.

4. Run Prisma migrations:

   
   npx prisma migrate dev --name init
   

### Running the Application

To start the server, run:


npm run dev


or


yarn dev


The application will be running on `http://localhost:4000`.

## API Documentation

### GraphQL Endpoints

You can interact with the GraphQL API using tools like [Postman](https://www.postman.com/) or [GraphQL Playground](https://www.graphql-playground.com/).

### Example Queries

- **Get all items**:

  
  query {
    items {
      id
      name
      description
    }
  }
  

- **Create a new item**:

  
  mutation {
    createItem(data: { name: "New Item", description: "Item Description" }) {
      id
      name
    }
  }
  

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

