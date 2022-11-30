# HAQAN-WAREHOUSE-PROJECT-
/*
 * To change this template, choose Tools | Templates
 * and open the template in the editor.
 */
package javaapplication47;

import java.util.Scanner;

class Warehouse{
    private String name;
    private String address;

    public Warehouse(String name, String address) {
        this.name = name;
        this.address = address;
    }

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public String getAddress() {
        return address;
    }

    public void setAddress(String address) {
        this.address = address;
    }
    
    
    public void addWarehouse(String name,String Address){
        this.name=name;
        this.address=Address;
        // add warehouse using name, address as inpout
    }
    
    public void printDetails(){
        System.out.print("******Warehouse's Detail******");

        System.out.println("\nAddress :"+getAddress()+"\nName :"+getName());
        // print details of warehouse here
    }
}


class Manager{
    private String name;
    private String Phone;
    private String Email;

    public Manager(String name, String Phone, String Email) {
        this.name = name;
        this.Phone = Phone;
        this.Email = Email;
    }

    

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public String getPhone() {
        return Phone;
    }

    public void setPhone(String Phone) {
        this.Phone = Phone;
    }

    public String getEmail() {
        return Email;
    }

    public void setEmail(String Email) {
        this.Email = Email;
    }
    
    
    public void displayDetails(){
System.out.println("******Manager's Detail******");
        System.out.println("Manager Name :"+getName()+"\nManager Phone :"+getPhone()+
                "\nManager Email :"+getEmail());
    }
}




class Order{
    private int FoodId;
    private String FoodName;
    private int quantity;

    public Order(int FoodId, String FoodName, int quantity) {
        this.FoodId = FoodId;
        this.FoodName = FoodName;
        this.quantity = quantity;
    }
    

    public int getFoodId() {
        return FoodId;
    }

    public void setFoodId(int FoodId) {
        this.FoodId = FoodId;
    }

    public String getFoodName() {
        return FoodName;
    }

    public void setFoodName(String FoodName) {
        this.FoodName = FoodName;
    }

    public int getQuantity() {
        return quantity;
    }

    public void setQuantity(int quantity) {
        this.quantity = quantity;
    }
    
    
    public void addOrder(){
        System.out.print("Order Added");
    }
    
    public void printOrderDetails(){
        System.out.println("*****Order Details*****");
      System.out.println("Food Id :"+getFoodId()+"\nFood Name :"+getFoodName()+
              "\nQuanitity :"+getQuantity());
    }
}




class Food{
    private int id;
    private String name;
    private String ExpiryDate;
    private int quantity;
    private String type;

    public Food(int id, String name, String ExpiryDate, int quantity, String type) {
        this.id = id;
        this.name = name;
        this.ExpiryDate = ExpiryDate;
        this.quantity = quantity;
        this.type = type;
    }

    
    public int getId() {
        return id;
    }

    public void setId(int id) {
        this.id = id;
    }

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public String getExpiryDate() {
        return ExpiryDate;
    }

    public void setExpiryDate(String ExpiryDate) {
        this.ExpiryDate = ExpiryDate;
    }

    public int getQuantity() {
        return quantity;
    }

    public void setQuantity(int quantity) {
        this.quantity = quantity;
    }

    public String getType() {
        return type;
    }

    public void setType(String type) {
        this.type = type;
    }
    
    
    public void printDetails(){
        // Details of food
        System.out.print("*****Food Details*****");
        System.out.println("Food Id :"+getId()+"\nFood Name :"+getName()+"\nExpiry Date :"
                +getExpiryDate()+"\nType :"+getType());
    }
}


class GroundStaff{
    private int id;
    private int sal;
    
    GroundStaff(int i, int s){
        id=i;
        sal=s;
    }

    public int getId() {
        return id;
    }

    public void setId(int id) {
        this.id = id;
    }

    public int getSal() {
        return sal;
    }

    public void setSal(int sal) {
        this.sal = sal;
    }
    
    
    public void showDetails(){
       System.out.print("Staff Id :"+getId()+"\nStaff Salary :"+getSal());
    }
}

public class JavaApplication47 {

    public static void main(String[] args) {
        // TODO code application logic here
        
        // create warehouse, order, food, manager, ground staff object here
        // and then add them respectively using there functions and then print their details 
    Warehouse w= new Warehouse("Haqan's Warehouse","DGKHAN");
    w.printDetails();
    Manager m=new Manager("Haqan","0345372372","Haqan@gmail.com");
    m.displayDetails();
    Order order= new Order(1,"Zinger Burger",5);
    order.printOrderDetails();
    Food f= new Food(1,"Zinger Burger","5/12/2022" , 5, "Fast");
    
    f.printDetails();
        
    }
    }
    
    
