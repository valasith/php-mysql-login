# PHP Login System
## Login Page
![login](https://user-images.githubusercontent.com/11474426/78792976-06ad2d00-79dc-11ea-99fe-a59c67662498.PNG)
>username: admin<br/>
>password: admin

## Home Page
![home](https://user-images.githubusercontent.com/11474426/78792478-5b9c7380-79db-11ea-86cf-bc2dfdb1f905.PNG)


## Profile Page
![profile](https://user-images.githubusercontent.com/11474426/78792508-648d4500-79db-11ea-836c-9a2cbc4094bb.PNG)
<hr>

# Creating the Database Table
```
CREATE TABLE `users` (
  `id` int(11) NOT NULL,
  `username` varchar(50) NOT NULL,
  `password` varchar(255) NOT NULL,
  `email` varchar(100) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8;

INSERT INTO `users` (`id`, `username`, `password`, `email`) VALUES
(1, 'admin', '$2y$10$cAtEsMzdM8KbWZEXmitlmuN.fVTZ9L3Up3iaelrB7DuMWItxOhsu6', 'admin@example.com');

ALTER TABLE `users`
  ADD PRIMARY KEY (`id`);

ALTER TABLE `users`
  MODIFY `id` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=2;
COMMIT;
```


