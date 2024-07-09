var assert = chai.assert;
assert(foo) // will pass for any truthy value (!= null,!= undefined,!= '',!= 0)
// or
assert(foo != null)
// or
assert.notEqual(foo, null);
