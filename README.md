# MobileDeviceDevelopment
//exc1
export default function calculateBMI(weight, height) {
    const bmi = weight / (height * height);
    let category;
  
    if (bmi < 18.5) {
      category = 'Underweight';
    } else if (bmi >= 18.5 && bmi <= 24.9) {
      category = 'Normal Weight';
    } else if (bmi >= 25 && bmi <= 29.9) {
      category = 'Overweight';
    } else if (bmi >= 30) {
      category = 'Obese';
    }
  
    return { bmi, category };
  }

// exc 2

    import calculateBMI from './index.js';

       const weight = 70;
       const height = 1.7;

       const result = calculateBMI(weight, height);
       console.log(`BMI: ${result.bmi}`);
       console.log(`Category: ${result.category}`);
       
       
