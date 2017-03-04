# APIs and JSON Serializing

What is the code that makes your JSON serializer return camelCase property names?

What is one way to fix your JSON serializer when you have a many to many relationship like this:

```csharp
    public class Cohort 
    {
        public virtual Instructor PrimaryInstructor { get; set; }
        public virtual List<Instructor> JuniorInstructors { get; set; }
        public virtual List<Student> Students { get; set; }
    }

    public class Instructor 
    {
        public virtual List<Cohort> Cohorts { get; set; }
    }

    //there is a many-to-many relationship between instructors and cohorts.
    //this relationship can cause an error during serialization because there's
    //a circular reference - A cohort has an instructor who has a cohort who has an instructor etc. etc.
```

