# Xunit assertions 

Commit: [c27a91f8cbcee37cb45699a3a81287bca225e876](https://github.com/xunit/xunit/tree/c27a91f8cbcee37cb45699a3a81287bca225e876)

## Summary

<details><summary>Boolean asserts</summary>

  - [True](#true)
  - [False](#false)

</details>

<details><summary>Collection asserts</summary>

  - [All](#all)
  - [AllAsync](#all-async)
  - [Collection](#collection)
  - [CollectionAsync](#collection-async)
  - [Contains](#contains)
  - [Distinct](#distinct)
  - [DoesNotContain](#does-not-contain)
  - [Empty](#empty)
  - [NotEmpty](#not-empty)
  - [Single](#single)

</details>

<details><summary>Equality asserts</summary>

  - [Equal](#equal)
  - [StrictEqual](#strict-equal)
  - [NotEqual](#not-equal)
  - [NotStrictEqual](#not-strict-equal)

</details>

<details><summary>Equivalence asserts</summary>
  
  - [Equivalent](#equivalent)

</details>

<details><summary>Event asserts</summary>

  - [Raises](#raises)
  - [RaisesAny](#raises-any)
  - [RaisesAsync](#raises-async)
  - [RaisesAnyAsync](#raises-any-async)

</details>

<details><summary>Exception asserts</summary>

  - [Throws](#throws)
  - [ThrowsAsync](#throws-async)
  - [ThrowsAny](#throws-any)
  - [ThrowsAnyAsync](#throws-any-async)

</details>

<details><summary>Fail asserts</summary>

  - [Fail](#fail)

</details>

<details><summary>Identity asserts</summary>

  - [Same](#same)
  - [NotSame](#not-same)

</details>

<details><summary>Multiple asserts</summary>

  - [Multiple](#multiple)

</details>

<details><summary>Null asserts</summary>

  - [Null](#null)
  - [NotNull](#not-null)

</details>

<details><summary>Property asserts</summary>

  - [PropertyChanged](#property-changed)
  - [PropertyChangedAsync](#property-changed-async)

</details>

<details><summary>Range asserts</summary>

  - [InRange](#in-range)
  - [NotInRange](#not-in-range)

</details>

<details><summary>Set asserts</summary>

  - [Subset](#subset)
  - [ProperSubset](@proper-subset)
  - [Superset](#superset)
  - [ProperSuperset](#proper-superset)

</details>

<details><summary>Skip asserts</summary>

  - [Skip](#skip)
  - [SkipUnless](#skip-unless)
  - [SkipWhen](#skip-when)

</details>

<details><summary>String/Span/Memory asserts</summary>

  - [StartsWith](#starts-with)
  - [EndsWith](#ends-with)

</details>

<details><summary>Regex asserts</summary>

  - [Matches](#matches)
  - [DoesNotMatch](#does-not-match)

</details>

<details><summary>Type asserts</summary>

  - [IsAssignableFrom](#is-assignable-from)
  - [IsNotType](#is-not-type)
  - [IsType](#is-type)

</details>
<hr/><br/>

## Boolean asserts

<a id="true"></a>

`Assert.True(expression)`

  - [TrueTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v1.tests/xunit/TrueTests.cs)
  - [BooleanAssertsTests/True](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/BooleanAssertsTests.cs#L58)

<a id="false"></a>

`Assert.False(expression)`

  - [FalseTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v1.tests/xunit/FalseTests.cs)
  - [BooleanAssertsTests/False](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/BooleanAssertsTests.cs#L7)

## Collection asserts

<a id="all"></a>

`Assert.All<T>(collection, predicate)`

`Assert.All(collection, predicate)`

  - [CollectionAssertsTests/All](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L16)

<a id="all-async"></a>

`Assert.AllAsync<T>(collection, predicate)`

`Assert.AllAsync(collection, predicate)`

  - [CollectionAssertsTests/AllAsync](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L89)

<a id="collection"></a>

`Assert.Collection(collection)`

`Assert.Collection(collection, predicate1, ..., predicateN)`

  - [CollectionAssertsTests/Collection](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L182)

<a id="collection-async"></a>

`Assert.CollectionAsync(collection)`

`Assert.CollectionAsync(collection, predicate1, ..., predicateN)`

  - [CollectionAssertsTests/CollectionAsync](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L254)

<a id="contains"></a>

`Assert.Contains(element, collection)`

`Assert.Contains(element, collection, comparer)`

`Assert.Contains(collection, predicate)`

`Assert.Contains<T>(collection, predicate)`

  - [CollectionAssertsTests/Contains](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L342)

  - [CollectionAssertsTests/Contains_WithComparer](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L477)

  - [CollectionAssertsTests/Contains_WithPredicate](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L521)

<a id="distinct"></a>

`Assert.Distinct(collection)`

`Assert.Distinct<T>(collection)`

`Assert.Distinct(collection, comparer)`

  - [CollectionAssertsTests/Distinct](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L547)

<a id="does-not-contain"></a>

`Assert.DoesNotContain(element, collection)`

`Assert.DoesNotContain(element, collection, comparer)`

`Assert.DoesNotContain(collection, predicate)`

  - [CollectionAssertsTests/DoesNotContain](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L613)

  - [CollectionAssertsTests/DoesNotContain_WithComparer](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L765)

  - [CollectionAssertsTests/DoesNotContain_WithPredicate](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L802)

<a id="empty"></a>

`Assert.Empty(collection)`

  - [CollectionAssertsTests/Empty](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L828)

<a id="not-empty"></a>

`Assert.NotEmpty(collection)`

  - [CollectionAssertsTests/NotEmpty](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L1083)

<a id="single"></a>

`Assert.Single(collection)`

`Assert.Single<T>(collection)`

`Assert.Single(collection, element)`

`Assert.Single(collection, predicate)`

`Assert.Single<T>(collection, predicate)`

  - [CollectionAssertsTests/Single_NonGeneric](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L1170)

  - [CollectionAssertsTests/Single_NonGeneric_WithObject](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L1222)

  - [CollectionAssertsTests/Single_Generic](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L1269)

  - [CollectionAssertsTests/Single_Generic_WithPredicate](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L1320)

## Equality asserts

<a id="equal"></a>

`Assert.Equal(expected, actual)`

`Assert.Equal<T>(expected, actual)`

`Assert.Equal(expected, actual, comparer)`

`Assert.Equal(expected, actual, precision)`

`Assert.Equal(expected, actual, precision, MidpointRounding)`

`Assert.Equal(expected, actual, tolerance)`

  - [CollectionAssertsTests/Equal](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L879)

  - [CollectionAssertsTests/Equal_WithComparer](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L1057)

  - [EqualityAssertsTests/Equal](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EqualityAssertsTests.cs#L11)

  - [EqualityAssertsTests/Equal_WithComparer](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EqualityAssertsTests.cs#L732)

  - [EqualityAssertsTests/Equal_Decimal](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EqualityAssertsTests.cs#L763)

  - [EqualityAssertsTests/Equal_Double](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EqualityAssertsTests.cs#L780)

  - [EqualityAssertsTests/Equal_Double_MidPointRounding](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EqualityAssertsTests.cs#L810)

  - [EqualityAssertsTests/Equal_Double_Tolerance](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EqualityAssertsTests.cs#L833)

  - [EqualityAssertsTests/Equal_Float](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EqualityAssertsTests.cs#L900)

<a id="strict-equal"></a>

`Assert.StrictEqual(expected, actual)`

  - [EqualityAssertsTests/StrictEqual](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EqualityAssertsTests.cs#L967)

<a id="not-equal"></a>

`Assert.NotEqual(expected, actual)`

`Assert.NotEqual(expected, actual, comparer)`

`Assert.NotEqual(expected, actual, precision)`

  - [CollectionAssertsTests/NotEqual](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L1114)

  - [CollectionAssertsTests/NotEqual_WithComparer](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/CollectionAssertsTests.cs#L1135)

  - [EqualityAssertsTests/NotEqual](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EqualityAssertsTests.cs#L1001)

  - [EqualityAssertsTests/NotEqual_WithComparer](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EqualityAssertsTests.cs#L1122)

  - [EqualityAssertsTests/NotEqual_Decimal](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EqualityAssertsTests.cs#L1146)

  - [EqualityAssertsTests/NotEqual_Double](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EqualityAssertsTests.cs#L1168)

<a id="not-strict-equal"></a>

`Assert.NotStrictEqual(expected, actual)`

  - [EqualityAssertsTests/NotStrictEqual](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EqualityAssertsTests.cs#L1190)

## Equivalence asserts

<a id="equivalent"></a>

`Assert.Equivalent(expected, actual)`

<code>Assert.Equivalent(expected, actual, strict: _boolean_)</code>

  - [EquivalenceAssertsTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EquivalenceAssertsTests.cs#L8)

## Event asserts

<a id="raises"></a>

`Assert.Raises<T>(predicate1, predicate2, predicate3)`

  - [EventAssertsTests/Raises_Generic](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EventAssertsTests.cs#L8)

<a id="raises-any"></a>

`Assert.RaisesAny<T>(predicate1, predicate2, predicate3)`

  - [EventAssertsTests/RaisesAny_Generic](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EventAssertsTests.cs#L59)

<a id="raises-async"></a>

`Assert.RaisesAsync<T>(predicate1, predicate2, predicate3)`

  - [EventAssertsTests/RaisesAsync_Generic](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EventAssertsTests.cs#L162)

<a id="raises-any-async"></a>

`Assert.RaisesAnyAsync<T>(predicate1, predicate2, predicate3)`

  - [EventAssertsTests/RaisesAnyAsync_Generic](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/EventAssertsTests.cs#L109)

## Exception asserts

<a id="throws"></a>

`Assert.Throws<E>(predicate)`

`Assert.Throws(exceptionType, predicate)`

`Assert.Throws<E>(paramName, predicate)`

<a id="throws-async"></a>

`Assert.ThrowsAsync<E>(predicate)`

`Assert.ThrowsAsync(exceptionType, predicate)`

`Assert.ThrowsAsync<E>(paramName, predicate)`

<a id="throws-any"></a>

`Assert.ThrowsAny<E>(predicate)`

<a id="throws-any-async"></a>

`Assert.ThrowsAnyAsync<E>(predicate)`

  - [ExceptionAssertsTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/ExceptionAssertsTests.cs#L7)

## Fail asserts

<a id="fail"></a>

`Assert.Fail(message)`

  - [FailAssertsTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/FailAssertsTests.cs#L5)

## Identity asserts

<a id="same"></a>

`Assert.Same(expected, actual)`

  - [SameTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v1.tests/xunit/SameTests.cs)

  - [IdentityAssertsTests/Same](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/IdentityAssertsTests.cs#L26)  

<a id="not-same"></a>

`Assert.NotSame(expected, actual)`

  - [NotSameTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v1.tests/xunit/NotSameTests.cs)

  - [IdentityAssertsTests/NotSame](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/IdentityAssertsTests.cs#L6)

## Multiple asserts

<a id="multiple"></a>

`Assert.Multiple()`

`Assert.Multiple(predicate1, ..., predicateN)`

  - [MultipleAssertsTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/MultipleAssertsTests.cs)

## Null asserts

<a id="null"></a>

`Assert.Null(expression)`

  - [NullTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v1.tests/xunit/NullTests.cs)

  - [NullAssertsTests/Null](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/NullAssertsTests.cs#L25)

<a id="not-null"></a>

`Assert.NotNull(expression)`

  - [NotNullTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v1.tests/xunit/NotNullTests.cs)

  - [NullAssertsTests/NotNull](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/NullAssertsTests.cs#L7)

## Property asserts

<a id="propert-changed"></a>

`Assert.PropertyChanged(element, property, predicate)`

  - [PropertyChangedTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v1.tests/xunit/PropertyChangedTests.cs)

  - [PropertyAssertsTests/PropertyChanged](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/PropertyAssertsTests.cs#L9)

<a id="property-changed-async"></a>

`Assert.PropertyChangedAsync(element, property, predicate)`

  - [PropertyAssertsTests/PropertyChangedAsync](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/PropertyAssertsTests.cs#L80)

## Range asserts

<a id="in-range"></a>

`Assert.InRange(value, minRange, maxRange)`

`Assert.InRange(value, minRange, maxRange, comparer)`

  - [InRangeTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v1.tests/xunit/InRangeTests.cs)

  - [RangeAssertsTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/RangeAssertsTests.cs)

<a id="not-in-range"></a>

`Assert.NotInRange(value, minRange, maxRange)`

`Assert.NotInRange(value, minRange, maxRange, comparer)`

  - [NotInRangeTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v1.tests/xunit/NotInRangeTests.cs)

  - [RangeAssertsTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/RangeAssertsTests.cs)

## Set asserts

<a id="subset"></a>

`Assert.Subset(expected, actual)`

  - [SetAssertsTests/Subset](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/SetAssertsTests.cs#L8)

<a id="proper-subset"></a>

`Assert.ProperSubset(expected, actual)`

  - [SetAssertsTests/ProperSubset](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/SetAssertsTests.cs#L52)

<a id="superset"></a>

`Assert.Superset(expected, actual)`

  - [SetAssertsTests/Superset](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/SetAssertsTests.cs#L96)

<a id="proper-superset"></a>

`Assert.ProperSuperset(expected, actual)`

  - [SetAssertsTests/ProperSuperset](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/SetAssertsTests.cs#L140)

## Skip asserts

<a id="skip"></a>

`Assert.Skip(testExpression)`

<a id="skip-unless"></a>

`Assert.SkipUnless(boolExpression, testExpression)`

<a id="skip-when"></a>

`Assert.SkipWhen(boolExpression, testExpression)`

  - [SkipAssertsTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/SkipAssertsTests.cs)

## String/Span/Memory asserts

<a id="starts-with"></a>

`Assert.StartsWith(search, text)`

`Assert.StartsWith(search, text, comparison)`

<a id="ends-with"></a>

`Assert.EndsWith(search, text)`

`Assert.EndsWith(search, text, comparison)`

  - [MemoryAssertsTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/MemoryAssertsTests.cs)

  - [SpanAssertsTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/SpanAssertsTests.cs)

  - [StringAssertsTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/StringAssertsTests.cs)

## Regex asserts

<a id="matches"></a>

`Assert.Matches(match, text)`

<a id="does-not-match"></a>

`Assert.DoesNotMatch(match, text)`

  - [StringAssertsTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v3.assert.tests/Asserts/StringAssertsTests.cs)

## Type asserts

<a id="is-assignable-from"></a>

`Assert.IsAssignableFrom(type, expression)`

`Assert.IsAssignableFrom<T>(expression)`

  - [IsAssignableFromTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v1.tests/xunit/IsAssignableFromTests.cs)

<a id="is-not-type"></a>

`Assert.IsNotType(type, expression)`

`Assert.IsNotType<T>(expression)`

  - [IsNotTypeTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v1.tests/xunit/IsNotTypeTests.cs)

<a id="is-type"></a>

`Assert.IsType(type, expression)`

`Assert.IsType<T>(expression)`

  - [IsTypeTests](https://github.com/xunit/xunit/blob/c27a91f8cb/src/xunit.v1.tests/xunit/IsTypeTests.cs)
