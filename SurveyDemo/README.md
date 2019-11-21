






<?= SurveyDev::widget([
    'id' => 'self-feedback',
	'questions' => ['C','C++ 'Java','Php','Jquery','python','Ruby'],
	'scale' => ['min' => 0, 'max' => 3],
	'sections' => ['Sep 2019 Estimation', 'Oct 2019 Estimation','Nov 2019 Estimation'],
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