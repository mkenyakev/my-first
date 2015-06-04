# my-first

<?php

class TestClass {
	public function __call($name, $arg) {
		call_user_func($name, $arg);
	}
}
class test {
	public function newTest() {

		function bigTest() {
			echo 'Big Test Here';
		}
		function smallTest() {
			echo 'Small Test Here';
		}

		$obj = new TestClass;

		return $obj;
	}

}
$rentry = new test;
$rentry->newTest()->bigTest();

