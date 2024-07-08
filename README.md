var chai = require('chai');
var assert = chai.assert;

suite('Unit Tests', function(){
  
  // Make ALL tests pass
  // !! Don't scramble the Assertions. We rely on their order to check the results !!
  suite('Basic Assertions', function() {
    /** assert.fail() will always fail. Change it into something more useful... **/
  
    /** 1 - Use assert.isNull() or assert.isNotNull() to make the tests pass. **/
    test('#isNull, #isNotNull', function(){
      assert.isNull(null, 'this is an optional error description - e.g. null is null');
      assert.isNotNull( 1, '1 is not null');
    });
  
    /** 2 - Use assert.isDefined() or assert.isUndefined() to make the tests pass. **/
    test('#isDefined, #isUndefined', function(){
      assert.isDefined( null, 'null is not undefined');
      assert.isUndefined( undefined, 'undefined IS undefined');
      assert.isDefined( 'hello', 'a string is not undefined' );
    });
  
    /** 3 - Use assert.isOk() or assert.isNotOk() to make the tests pass. **/
    // .isOk(truthy) and .isNotOk(falsey) will pass
    test('#isOk, #isNotOk', function(){
      assert.isNotOk( null, 'null is falsey');
      assert.isOk( "I'm truthy", 'a string is truthy');
      assert.isOk( true, 'true is truthy' );
    });
