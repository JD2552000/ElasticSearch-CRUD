# ElasticSearch-CRUD
Implemented CRUD operations with ElasticSearch

Steps to SetUp and Run the App:-

Step1:-  Install ElasticSearch for database usuage.
Step2:-  Create student indexes using elasticsearch

Step3:- Insert some data to check whether we are able to fetch it using query.
Step4:- Implement utility function for connecting to a database and executing the query.
Step5:- Implement CRUD function to create update read and delete student.
Step6:- Implement Endpoint for each operations having different usuage.
Step7:- To run the application in IDE go to the terminal containing the file and apply below command to the
        app will run as a localhost connected to DB.
        Command:- uvicorn main:app --reload
Step8:- Install Postman as a tool to run the endpoints and check whether we are able to implement CRUD operations and url and body
        for the request are as follows:-
        GET ALL API:- 
            URL:- http://localhost:8000/students/
        GET BY ID API:- 
            URL:- http://localhost:8000/students/1
        POST API:- 
            URL:- http://localhost:8000/students/
            BODY:- {
                        "name": "Dikshant",
                        "age": 24,
                        "grade": "A"
                    }
        PUT API:-
            URL:- http://localhost:8000/students/2
            BODY:- {
                        "name": "Dikshant P",
                        "age": 23,
                        "grade": "A+"
                    }
        DELETE API:-
            URL:- http://localhost:8000/students/1
