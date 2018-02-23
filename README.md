# sum
sum function!

const sumFunction = (...args) => verify(args)
const verify = function (args) {
  const veryfied = args.map(val => {
    if (typeof val === 'number' && !isNaN(val)) {
      return val
    } else return false
  })
  return veryfied.reduce((zero, num) => zero + num, 0)
}

console.log(sumFunction(17, 3, 8, [], true, '18'))	// 28
