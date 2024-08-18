<script setup>
   import { defineProps } from 'vue'

   defineProps({
     task: Object
   })
</script>

<template>
    <div class="task-container">
        <!-- Task Card 1 -->
        <div class="job-card">
            <div class="content">
                <div class="job-info">
                    <div class="job-type">Routine</div>
                    <h3 class="job-title">Morning Exercise</h3>
                </div>

                <div class="job-description">
                    30 minutes of jump roping followed by 20 push-ups. Focus on maintaining a consistent pace and form.
                </div>

                <h3 class="job-salary">2024-08-18 / 07:00 AM - 07:45 AM</h3>

                <div class="separator"></div>

                <div class="job-footer">
                    <div class="job-location">
                        <i class="fa-solid fa-location-dot"></i> High
                    </div>
                    <a href="/job/id" class="read-more">Read More</a>
                </div>
            </div>
        </div>

        <!-- Task Card 2 -->
        <div class="job-card">
            <div class="content">
                <div class="job-info">
                    <div class="job-type">Routine</div>
                    <h3 class="job-title">Morning Exercise</h3>
                </div>

                <div class="job-description">
                    30 minutes of jump roping followed by 20 push-ups. Focus on maintaining a consistent pace and form.
                </div>

                <h3 class="job-salary">2024-08-18 / 07:00 AM - 07:45 AM</h3>

                <div class="separator"></div>

                <div class="job-footer">
                    <div class="job-location">
                        <i class="fa-solid fa-location-dot"></i> High
                    </div>
                    <a href="/job/id" class="read-more">Read More</a>
                </div>
            </div>
        </div>

        <!-- Task Card 3 -->
        <div class="job-card">
            <div class="content">
                <div class="job-info">
                    <div class="job-type">Routine</div>
                    <h3 class="job-title">Morning Exercise</h3>
                </div>

                <div class="job-description">
                    30 minutes of jump roping followed by 20 push-ups. Focus on maintaining a consistent pace and form.
                </div>

                <h3 class="job-salary">2024-08-18 / 07:00 AM - 07:45 AM</h3>

                <div class="separator"></div>

                <div class="job-footer">
                    <div class="job-location">
                        <i class="fa-solid fa-location-dot"></i> High
                    </div>
                    <a href="/job/id" class="read-more">Read More</a>
                </div>
            </div>
        </div>
        <!-- Task Card 4 -->
        <div class="job-card">
            <div class="content">
                <div class="job-info">
                    <div class="job-type">Routine</div>
                    <h3 class="job-title">Morning Exercise</h3>
                </div>

                <div class="job-description">
                    30 minutes of jump roping followed by 20 push-ups. Focus on maintaining a consistent pace and form.
                </div>

                <h3 class="job-salary">2024-08-18 / 07:00 AM - 07:45 AM</h3>

                <div class="separator"></div>

                <div class="job-footer">
                    <div class="job-location">
                        <i class="fa-solid fa-location-dot"></i> High
                    </div>
                    <a href="/job/id" class="read-more">Read More</a>
                </div>
            </div>
        </div>
    </div>
</template>

<style>
/* Container for task cards */
.task-container {
    padding: 40px;
    background-color: rgb(187, 167, 167);
    display: grid;
    grid-template-columns: repeat(1, 1fr);
    gap: 24px; /* 24px gap between columns */
}

@media (min-width: 768px) {
    .task-container {
        grid-template-columns: repeat(3, 1fr); /* 3 columns for larger screens */
    }
}

/* Styling for the job card container */
.job-card {
    background-color: rgb(247, 220, 220);
    border-radius: 10px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    position: relative;
    margin-bottom: 24px; /* Add space at the bottom */
}

/* Styling for the inner content */
.content {
    padding: 16px;
}

/* Job info container */
.job-info {
    margin-bottom: 24px;
}

/* Job type text */
.job-type {
    color: #718096; /* Equivalent to text-gray-600 */
    margin-bottom: 8px;
}

/* Job title styling */
.job-title {
    font-size: 1.25rem; /* Equivalent to text-xl */
    font-weight: bold;
}

/* Job description styling */
.job-description {
    margin-bottom: 20px;
}

/* Job salary styling */
.job-salary {
    color: #462e2e; /* Equivalent to text-green-500 */
    margin-bottom: 8px;
}

/* Separator line */
.separator {
    border: 1px solid #edf2f7; /* Equivalent to border-gray-100 */
    margin-bottom: 20px;
}

/* Footer container for location and read more link */
.job-footer {
    display: flex;
    flex-direction: column; /* Default to column for small screens */
    justify-content: space-between;
    margin-bottom: 16px;
}

@media (min-width: 1024px) {
    .job-footer {
        flex-direction: row; /* Row direction for larger screens */
    }
}

/* Job location styling */
.job-location {
    color: #dd6b20; /* Equivalent to text-orange-700 */
    margin-bottom: 12px;
    font-size: 1rem; /* Equivalent to text-lg */
}

/* Read more link styling */
.read-more {
    display: inline-block;
    height: 36px;
    background-color: #472a2a; /* Equivalent to bg-green-500 */
    color: white;
    padding: 8px 16px;
    border-radius: 8px;
    text-align: center;
    font-size: 0.875rem; /* Equivalent to text-sm */
    text-decoration: none;
    transition: background-color 0.3s ease;
}

.read-more:hover {
    background-color:  #6e4141; /* Equivalent to hover:bg-green-600 */
}
</style>
