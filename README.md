# hello-world
This is not a pipe.


//
//  Daughter.swift
//  playgroundApp-1
//
//  Created by Mike on 3/17/18.
//  Copyright © 2018 BummerBro. All rights reserved.
//

import Foundation

class Daughter {
	var name: String
	var age: Int
	var personality: String
	var ageWillMoveOut: Int = 18
	
	
	// define getter and setter for age daughter will move out and years left in house
	
	var yearsLeftInHouse: Int {
		get {
			return ageWillMoveOut - age
		}
		set {
			ageWillMoveOut = age + newValue
		}
	}
	// give the Daughter class an initializer that calls for the properties
	
	init(name: String, age: Int, personality: String) {
		self.age = age
		self.name = name
		self.personality = personality
	}
	
	// set a method that describes the instance of Daughter that is instantiated
	
	func isLike() -> String {
		return "\(name) is a \(age) year old girl who is \(personality)."
	}
}
