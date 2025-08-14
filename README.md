# Practice Ground for OLAP

A **practice ground for OLAP principles** using PostgreSQL. This project helps learners write and experiment with complex **`SELECT` queries** and explore analytical SQL capabilities.

## Purpose

- This repository is designed for learners who want hands-on experience with OLAP queries in a real database setup.
- You can easily add your own scripts and run them inside a containerized PostgreSQL environment.


## Installation & Usage

### 1. Clone the Repository

```bash
git clone https://github.com/techatpark/rdbms-olap-practice.git
cd rdbms-olap-practice
```

---

### 2. Add Your Practice Scripts

Place your `.sql` files inside the `init/` directory.
These scripts will be automatically executed when the PostgreSQL container starts for the first time.

Example:

```bash
init/
  ├── sample_queries.sql
  ├── my_practice_1.sql
  └── my_practice_2.sql
```

---

### 3. Start the Environment

```bash
docker-compose up -d
```

Access Superset at: http://localhost:8088 with  credentials `admin / admin`


### 4. Configure Database

1. Go to `Settings > Database Connections`.
2. Add Database
3. Select Postgress with below values
     - Host: `postgres`
     - Port: `5432`
     - Database name: `superset_db`
     - Username: `superset_user`
     - Password: `superset_pass`
     - Click `Connect`
     - Click `Finish`

