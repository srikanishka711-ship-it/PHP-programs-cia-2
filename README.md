# PHP-programs-cia-2
Employee Age and Retirement Calculator
<!DOCTYPE html>
<html>
<body>

<h2>Employee Age and Retirement Calculator</h2>

<?php
$name = "Arun";
$dob = "15-06-1998";
$retirement_age = 60;

$birthDate = new DateTime($dob);
$today = new DateTime();

$age = $today->diff($birthDate)->y;
$remaining = $retirement_age - $age;

echo "Employee Name: $name<br>";
echo "Date of Birth: $dob<br>";
echo "Current Age: $age years<br>";

if ($remaining > 0)
    echo "Years Remaining for Retirement: $remaining years";
else
    echo "Employee has reached retirement age.";
?>

</body>
</html>
Output
Employee Age and Retirement Calculator

Employee Name: Arun
Date of Birth: 15-06-1998
Current Age: 28 years
Years Remaining for Retirement: 32 years

