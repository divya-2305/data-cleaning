To clean the Netflix titles dataset (netflix_titles.csv), we used pandas in Python to address missing values, duplicates, and inconsistent formats:

Missing Values: Filled missing director, cast, and country with 'Unknown', dropped rows with missing title, type, or date_added, and imputed missing rating with the mode.
Duplicates: Removed duplicate rows based on title and type, keeping the first occurrence (e.g., handled cases like "Tughlaq Durbar").
Inconsistent Formats: Standardized type to title case, parsed date_added into datetime, mapped inconsistent rating values (e.g., 'UR' to 'R'), cleaned country and listed_in for consistent comma-separated formatting, and converted movie duration to numeric minutes while retaining TV show durations as strings.
Output: Saved the cleaned dataset to cleaned_netflix_titles.csv after verifying with checks on missing values, duplicates, and data types.
