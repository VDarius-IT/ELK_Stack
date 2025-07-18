### Quick Start Guide

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
    cd YOUR-REPOSITORY
    ```

2.  **For a Quick Development Setup (No Security):**
    ```bash
    # This will use docker-compose.yml and logstash.conf
    docker-compose up -d
    ```

3.  **For a Production-Like Setup (With Security):**

    > **Important:** First, edit the passwords! Open `docker-compose.prod.yml` and change `YourStrongPasswordHere` to a secure password in all three places (Elasticsearch, Logstash, and Kibana).

    Then, run the stack using the production file:
    ```bash
    # This will use docker-compose.prod.yml and logstash.prod.conf
    docker-compose -f docker-compose.prod.yml up -d
    ```
