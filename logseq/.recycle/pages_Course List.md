public:: true

- # Core (Mandatory) Courses
	- {{query (and (page-property type course) (page-property course_type core) )}}
	  query-properties:: [:page :ects :quarter :created-at :updated-at]
	  query-table:: true
	  query-sort-by:: ects
	  query-sort-desc:: true
	-
- # Elective Courses
	- {{query (and (page-property type course) (page-property course-type elective) )}}
	  query-properties:: [:created-at :updated-at :page :ects :quarter]
	  query-sort-by:: quarter
	  query-sort-desc:: false
	  query-table:: true
-