# Practice2-Author

import java.lang.*;

public class Author {
    private char gender;
    private String name;
    private String email;

    public Author(String n, char g, String e) {
        name = n;
        email = e;
        gender = g;
    }

    public String getName() {
        return name;
    }

    public String getEmail() {
        return email;
    }

    public void setEmail(String email) {
        this.email = email;
    }
    public void setGender(char gender) {
        this.gender = gender;
    }

    public char getGender() {
        return gender;
    }

    public void setName(String name) {
        this.name = name;
    }
    public String toString(){
        return this.name + "(" + this.gender + ") " + "email is " + this.email;
    }
}


import java.lang.*;
public class TestAuthor {
    public static void main(String[] args) {
        Author a1 = new Author("Erich Fromm", 'M',"erichfrommik@gmal.mir");
        System.out.println(a1);
        a1.setEmail("erichfrommik@gmal.mir");
        System.out.println(a1);
        System.out.println(a1.getEmail());
    }
}
