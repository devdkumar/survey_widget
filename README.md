# survey_widget




<?= \SurveyDev::widget([
	'id' => 'self-feedback',
	'questions' => ['C','C++ 'Java','Php','Jquery','python','Ruby'],
	'scale' => ['min' => 0, 'max' => 5],
	'sections' => ['2015 Scores', '2016 Scores'],
	'enableComment' => true,
]); ?>



CREATE TABLE dev_survey (

id INT(6) UNSIGNED AUTO_INCREMENT PRIMARY KEY,
score VARCHAR(30) NOT NULL,
question_id int(30) NOT NULL,
comment VARCHAR(30) NOT NULL,
user_id int(30) NOT NULL,
reg_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP
)

CREATE TABLE dev_question (

id INT(6) UNSIGNED AUTO_INCREMENT PRIMARY KEY,
title VARCHAR(30) NOT NULL,
decsription int(30) NOT NULL,
reg_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP
)
