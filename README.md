# SDE Intern Assignment Chat360
Quality Log Control

[**Live**](https://logcontrolsoftware.netlify.app/)

## Backend Live to Enter logs
[**Live**](https://quality-log-backend.onrender.com)

### Steps to Enter post logs
- 1. Enter url https://quality-log-backend.onrender.com on postman or any software that you used. It is an API's
  2. It is an Post method so it requires body data
  3. - ```josn
       [
	    {
	        "level": "error",
	        "log_string": "Inside the Search API",
	        "timestamp": "2024-09-15T08:00:00Z",
	        "metadata": {
	            "source": "log3.log"
	        }
	    },
	    {
	        "level": "info",
	        "log_string": "User login successful",
	        "timestamp": "2024-09-16T09:30:00Z",
	        "metadata": {
	            "source": "log1.log"
	        }
	    },
	    {
	        "level": "success",
	        "log_string": "Data processed successfully",
	        "timestamp": "2024-09-17T10:45:00Z",
	        "metadata": {
	            "source": "log2.log"
	        }
	    }
       ]

## Objective

Build a problem solution that uses APIs with logs at different stages. These logs should be stored in some log files such as `log1.log`, `log2.log` etc files. 
You need to build a Query Interface also that traverses through these logs files and fetches logs based on timestamp, log string, source of the log, etc.
Both the systems (the log stores and the query interface) can be built using any programming language of your choice.

## Sample Log Data Format:

The logs might have the below format.

-
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

### Log Ingestor:

1. **API Integration:** Integrate 8-9 APIs into your application to capture logs at different stages. Ensure that each API can write logs to a designated file, such as `log1.log`, `log2.log`, and so on.
2. **Log Formatting:** Standardize the format for logging across all APIs. This could include a timestamp, log level, source, log message, etc.
3. **Logging Configuration:** Implement a mechanism to configure logging levels and file paths for each API. This could be through a configuration file or environment variables.
4. **Error Handling:** Implement robust error handling to ensure that failures in logging do not disrupt the application's functionality.

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

Total File Examined For Search Query On Level : "Err" is 47 , Here it is applying Linear Search

## File Examined When there is indexing in DB
Aim for efficient and quick search results.

Total File Examined For Search Query On Level : “Err” is 14 , Here it is applying Binary Search

#### Indexing Optimised the search query by Logarthmic Time Complexity

---

## Demo

Video Demo Here

## Required Software

- Node Js must be installed before running project
- MongoDB compass is helpful for view database collection

## Run Locally

Clone the project

```bash
  git clone https://github.com/bitleakash6/Qaulity_Log_Control_MERN_Project.git
```

Move into Project folder

```bash
cd Quality_Log_Control
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

## Authors

- [@AkashBitle](https://github.com/bitleakash6)

## Feedback

If you have any feedback, please reach out to us at akashbitle3@gmail.com
