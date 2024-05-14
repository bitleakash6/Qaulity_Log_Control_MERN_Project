# SDE Intern Assignment Chat360
Quality Log Control

## Objective

Build a problem solution that uses APIs with logs at different stages. These logs should be stored in some log files such as `log1.log`, `log2.log` etc files. 
You need to build a Query Interface also that traverses through these logs files and fetches logs based on timestamp, log string, source of the log, etc.
Both the systems (the log stores and the query interface) can be built using any programming language of your choice.

- **Example:**
  ```json
  {
	"level": "error", ["info", "error", "success"]
	"log_string": "Inside the Search API",
	"timestamp": "2023-09-15T08:00:00Z",    
    "metadata": {
        "source": "log3.log"
    }
  }


## Tech Stack

*Client:* React.Js, Redux, Material UI

*Server:* Node.Js, Express.Js ,Mongodb

## Features Implemented

#### 1. Mechanism for Log Ingestion

- Implement a robust mechanism to ingest logs in the specified JSON format.

#### 2. Scalability

- Ensure the system's scalability to handle high volumes of logs efficiently.

#### 4. HTTP Server for Ingestion

- Logs should be ingested via an HTTP server running on the default port '3000'

## Bonus Features Implemented

#### 1. Search within Specific Date Ranges

- Enhance the log ingestor to support searching within specific date ranges, providing more flexibility for querying.

#### 2. Real-Time Log Ingestion

- Implement real-time log ingestion capabilities, ensuring that logs are processed and made available for querying in real-time.

#### 3. Regular Expression Support

- Extend the log ingestor to support search queries using regular expressions for more advanced log filtering.

#### 4. Combined Multiple Filters

- Allow users to combine multiple filters in a single query, enabling more complex and specific log searches.

#### 5. Role-Based Access

- Implement role-based access control to the log ingestor, restricting access based on user roles for enhanced security.

---

### File Examined When there is no indexing in DB

![logind](https://github.com/AnuragRoshan/images/blob/main/notIndex.png)

Total File Examined For Search Query On Level : "Err" is 47 , Here it is applying Linear Search

## File Examined When there is indexing in DB

![logind2](https://raw.githubusercontent.com/AnuragRoshan/images/main/index.png)

Total File Examined For Search Query On Level : “Err” is 14 , Here it is applying Binary Search

#### Indexing Optimised the search query by Logarthmic Time Complexity

---

## Demo

Video Demo Here

https://drive.google.com/file/d/1yEWF9ce-nk-nmuk6jfYmPpPu9XFLyz4_/view?usp=sharing

## Required Software

- Node Js must be installed before running project
- MongoDB compass is helpful for view database collection

## Run Locally

Clone the project

```bash
  git clone https://github.com/AnuragRoshan/LogIngestor.git
```

Move into Project folder

```bash
cd november-2023-hiring-AnuragRoshan
```

Move into server and install node dependencies for server side

```bash
cd server
npm i
```

Install react dependencies in client folder

```bash
cd ..
cd client
npm i
```

Run node backend in other shell

```bash
npm start
```

Run react frontend in third shell

```bash
cd ..
cd client
npm start
```

## References

- MongoDB Official Documentation : https://www.mongodb.com/docs/
- Indexing On Database : https://youtu.be/yo6ZXsgsyBA?si=Ft5swjQ9MgU-TkPi
- Front End UI : https://devsnap.me/css-toggle-switches

## Authors

- [@AnuragRoshan](https://github.com/AnuragRoshan)

## Feedback

If you have any feedback, please reach out to us at anuragraushan373@gmail.com

## Toggle Role Page

![mvrs6](https://github.com/AnuragRoshan/images/blob/main/log1.png)

The "Toggle Role" page enables administrators to effortlessly switch between roles, granting access to specialized query filters. This streamlined interface empowers administrators with exclusive capabilities, ensuring users maintain restricted access without compromising security.

## Filter Page

![mvrse1](https://github.com/AnuragRoshan/images/blob/main/log2.png)

![mvrs9](https://github.com/AnuragRoshan/images/blob/main/log3.png)
