# JavaScript-Grade-Calculator
grade calculator function that takes the earned points and total possible points as arguments, and returns the score in a detailed string.

     const gradeCalc = function (earned, possible) {
      if (typeof earned !== 'number' || typeof possible !== 'number') {
        throw Error('please provide numbers only!')
    }
        const score = (earned / possible) * 100
        let letterGrade = ' ' //empty string is replaced in if statements & used in string templates
        if (score >= 90) {
            letterGrade = 'A' // letterGrade now = A
        } else if (score >= 80) {
            letterGrade = 'B'
        } else if (score >= 70) {
            letterGrade = 'C'
        } else if (score >= 60) {
            letterGrade = 'D'
        } else {
            letterGrade = 'F'
        }
        return `You got a ${letterGrade} (${score}%!)` //letterGrade values in string templates
      } 
