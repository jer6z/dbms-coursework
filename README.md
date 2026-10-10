Database Audit Logging and Intrusion Detection System (DB_IDS_Project)

Institution: Middle Tennessee State University — Department of Computer Science

Course: Database Security Course Project

Team Members: Jorge E. Rosario, Adam Gold, Alan Young
Project Abstract

The Database Audit Logging and Intrusion Detection System (db_ids_project) is a robust security framework designed to monitor, capture, and analyze database transactions and user sessions in real time. The system actively tracks suspicious database operations, evaluates transaction logs against predefined threshold rules, and generates immediate security alerts to mitigate unauthorized access and privilege escalation attempts.
System Architecture & Relational Schema

The database architecture is designed in Third Normal Form (3NF) to ensure data integrity, eliminate redundancy, and support high-performance audit querying.

    Users: Manages system user accounts, authentication identifiers, security roles, and account creation timestamps.

    DetectionRules: Stores intrusion detection rules, numeric threshold limits, evaluation time windows, and active status flags.

    SystemLogs: Captures raw system event logs, operation categories (e.g., login, query execution, data modification), execution status outcomes, raw query text, and origin IP addresses linked to user sessions.

    SecurityAlerts: Records security alert events generated when system log entries violate active detection rules, classifying alerts by severity and timestamp.

Core Functional Modules

    Audit Event Logging: Intercepts and records granular session details, tracking successful and failed connection attempts, statement executions, and administrative modifications.

    Rule-Based Anomaly Detection: Evaluates incoming system logs against sliding time-window thresholds (e.g., repeated login failures or unauthorized structural commands).

    Automated Alert Generation: Triggers high-priority security alerts linked directly to violating log entries and matched detection rules.

Repository Setup & Usage Instructions

To set up and run the database security environment:

    Database Initialization:
    Execute the core setup script to instantiate the relational schema, foreign key referential constraints, documentation comments, and seed data rows.

    Verification:
    Verify table creation and relational mapping integrity using your database management system console or command-line interface.

Project Status & Update Notice

    Current Status: Active Development and Architecture Verification.

    Update Statement: This repository and documentation will be continuously updated as new features, triggers, detection rules, and code changes are implemented throughout the project lifecycle.
