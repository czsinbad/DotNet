# DotNetWebcharting

#CREATE Procedure [dbo].[GetGdp]  
    (  
    @id int=null  
          )  
    as  
    begin  
    Select code,gdp from  cgdp 
    End 


#CREATE TABLE [dbo].[cgdp] 
(
 [Id]      INT          IDENTITY (1, 1) NOT NULL,
 [country] VARCHAR (50) NOT NULL,
 [code]    VARCHAR (3)  NULL,
 [gdp]     INT          DEFAULT ((0)) NOT NULL,
 PRIMARY KEY CLUSTERED ([Id] ASC)
);
