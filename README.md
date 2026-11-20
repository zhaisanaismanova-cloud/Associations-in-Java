# Java OOP Associations

This repository contains four Java examples demonstrating different types of associations between classes using object-oriented programming.

Each association demonstrates:
- At least one-to-many (`1 — *`) cardinality.
- Automatic reverse connection between related objects.
- Creating and removing relationships while keeping both sides synchronized.
**Project goal:** Demonstrate the implementation of different UML association types in Java, including cardinalities and automatic bidirectional relationship management.

## 1. Binary Association

A binary association represents a relationship between two classes.

**Example:** Game  and Character.

One game can have multiple characters, while each character belongs to one game.

## 2. Association with an Attribute

An association with an attribute is used when a relationship between two classes has its own attributes.

**Example:** Client, Dentist and Appointment.

The Appointment class connects a Client with a Dentist and stores information about the relationship, such as date, time, treatment type and price.

The original many-to-many relationship is transformed into two one-to-many associations.

## 3. Qualified Association

A qualified association uses a key (qualifier) to identify a specific object from a group of related objects.

**Example:** Customer and Country.

A country can have multiple customers, and countryCode is used as a qualifier to access customers belonging to a specific country.

## 4. Composition

Composition is a strong whole-part relationship in which the part depends on the lifetime of the whole.

**Example:** Contest and Contestant.

One contest can have many contestants. Each contestant belongs to one contest and cannot exist independently of it.

---

## Files
- `Main.java` - examples showing how each association is used with adding, deleting 
- binary folder with 2 classes
- withattribute folder with 3 classes
- composition folder with 2 classes
- qualified folder with 2 classes

## How to run
    javac *.java
    java Main

Requires Java 8 or newer.
