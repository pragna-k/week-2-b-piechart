# week-2-b-piechart
#Pie chart."
Names <- c("pragna","swathi","lohitha","nithya","bhuvana");
Rollno <- c("Y20CS093","Y20CS123","Y20CS095","Y20CS127","Y20CS130")
Gender <- c("Female","Female","Female","Female","Female")
Marks <-c(9,3,6,8,9)
Fee <-c(69400,57892,58903,69400,67390)
Section <-c("B","C","C","B","B")

rvrstudents <-data.frame(Names,Rollno,Gender,Marks,Fee,Section)
rvrstudents
write.csv(rvrstudents,"Rvr_Students.csv",row.names=F)

a <- read.csv("Rvr_Students.csv")



genere <- table(rvrstudents$Marks)
pie(genere,
    main="RVR&JC",
    border="blue",
    col=("Lavender")
)




OUTPUT:
> #Pie chart."
> Names <- c("Ujjwal","Satwika","Manya","Kiran","Subhiksha")
> Rollno <- c("Y20CS134","Y20CS145","Y20CS149","Y20CS127","Y20CS129")
> Gender <- c("Male","Female","Female","Male","Female")
> Marks <-c(9,3,6,8,9)
> Fee <-c(69400,57892,58903,69400,67390)
> Section <-c("B","C","C","B","B")
> rvrstudents <-data.frame(Names,Rollno,Gender,Marks,Fee,Section)
> rvrstudents
      Names   Rollno Gender Marks   Fee Section
1    pragna Y20CS093   Female     9 69400       B
2   Swathi Y20CS123 Female     3 57892       C
3     lohitha Y20CS095 Female     6 58903       C
4     nithya Y20CS127   Female     8 69400       B
5 bhuvana Y20CS30 Female     9 67390       B
> write.csv(rvrstudents,"Rvr_Students.csv",row.names=F)
> a <- read.csv("Rvr_Students.csv")
> genere <- table(rvrstudents$Marks)
> pie(genere,
+     main="RVR&JC",
+     border="blue",
+     col=("Lavender")
+ )
