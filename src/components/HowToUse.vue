<template>
    <div class="help-container">
        <!-- Help Section -->
        <div class="help">
            <h1>How To Use</h1>
            <h3>Welcome To The Daily Time Scheduler Help Page!</h3>
            <p>This page provides guidance on how to effectively use the Daily Task Scheduler to manage your daily activities and keep track of prior tasks.</p>
            <h3>Getting Started</h3>
            <h4>Add a New Task:</h4>
            <p>To create a new task, click on the "+" button located at the bottom-right corner of your screen. This will open a form where you can enter the task's name, description, start time, end time, and priority level. Once completed, click "Save" to add the task to your schedule.</p>
            <h4>View Your Schedule:</h4>
            <p>Your tasks for the day are displayed in a timeline format, organized by time slots. Each task appears as a card in its designated time slot. You can scroll through your schedule to see all planned activities for the day.</p>
            <h1>Thank You For Choosing DTS!</h1>
        </div>

    </div>
    <!-- Copyright Panel -->
    <div class="copyright-panel">
        <p>&copy; 2024 Daily Task Scheduler. All Rights Reserved.</p>
    </div>
</template>

<style>
/* Container for the help section and copyright panel */
.help-container {
    background-color: #412a2a; /* Brown background */
    color: white; /* White text for better readability */
    padding: 20px;
    border-radius: 10px;
}

/* Styling for the help section */
.help {
    margin-bottom: 20px;
}

/* Styling for the headers */
.help h1, .help h3, .help h4 {
    color: #f4f4f4; /* Light gray for headers */
}

/* Styling for the paragraphs */
.help p {
    color: #e0e0e0; /* Light gray for text */
    margin-bottom: 16px;
    line-height: 1.6;
}

/* Copyright panel styling */
.copyright-panel {
    background-color: #201816; /* Darker brown */
    padding: 10px;
    text-align: center;
    border-radius: 5px;
    margin-top: 20px;
}

/* Styling for the copyright text */
.copyright-panel p {
    margin: 0;
    color: #ffffff; /* White text */
    font-size: 0.875rem; /* Equivalent to text-sm */
}
</style>
