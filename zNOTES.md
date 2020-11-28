

=========== WARNING ===========
Lab opened with these warnings:

    npm WARN javascript-lab@1.0.0 No repository field.
npm WARN javascript-lab@1.0.0 license should be a valid SPDX license expression

added 233 packages from 654 contributors and audited 233 packages in 5.074s
found 166 vulnerabilities (164 low, 2 high)
  run `npm audit fix` to fix them, or `npm audit` for details
Done.
===============================


LAST LAB


Reference
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment

    Unpacking fields from objects passed as a function parameter
const user = {
  id: 42,
  displayName: 'jdoe',
  fullName: {
    firstName: 'John',
    lastName: 'Doe'
  }
};

function userId({id}) {
  return id;
}

function whois({displayName, fullName: {firstName: name}}) {
  return `${displayName} is ${name}`;
}

console.log(userId(user)); // 42
console.log(whois(user));  // "jdoe is John"



