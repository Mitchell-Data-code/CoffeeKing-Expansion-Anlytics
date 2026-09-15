# Count of coffee shops by star rating
SELECT 
  stars AS star_rating,
  COUNT(*) AS count_of_businesses
FROM yelp_academic_dataset_nash_business
WHERE categories LIKE '%Coffee & Tea%'
GROUP BY stars
ORDER BY stars
