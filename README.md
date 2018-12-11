# stockpricecalculator
CSV Files used are contained in StockPriceCalculator/FilesUpload

Initial Catalog in connectionString needs to be changed if database created has different name than provided.

A local server connection needs to established and exist for usage in Visual Studio.

Table names should be the same if the script below is used as well as datatypes.

Script: CREATE TABLE [dbo].[AppleInc] ( [Date] DATETIME NOT NULL, [Open] MONEY NOT NULL, [High] MONEY NOT NULL, 
[Low] MONEY NOT NULL, [Close] MONEY NOT NULL, [AdjClose] MONEY NOT NULL, [Volume] VARCHAR (50) NOT NULL, 
CONSTRAINT [PK_AppleInc] PRIMARY KEY CLUSTERED ([Date] ASC) );

CREATE TABLE [dbo].[SP500] ( [Date] DATETIME NOT NULL, [Open] MONEY NOT NULL, [High] MONEY NOT NULL, 
[Low] MONEY NOT NULL, [Close] MONEY NOT NULL, [AdjClose] MONEY NOT NULL, [Volume] VARCHAR (50) NOT NULL, 
CONSTRAINT [PK_SP500] PRIMARY KEY CLUSTERED ([Date] ASC) );
