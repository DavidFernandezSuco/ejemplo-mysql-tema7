
Vagrant.configure("2") do |config|
  
  config.vm.box = "ubuntu/xenial64"

  config.vm.provision "shell", inline: <<-SHELL

    #generar archivo SQL con los registros de empleados
    echo "--Insertar datos de ejemplo en la tabla 'empleados'" > /home/vagrant/datos_empleados.sql
    echo > "INSERT INTO gestion_empleados.empleados (nombre, apellido, edad, salario, departamento) 
    VALUES" >> /home/vagrant/datos_empleados.sql
    echo "('Juan', 'Perez', 30, 2500.00, 'Ventas')," >> /home/vagrant/datos_empleados.sql
    echo "('Ana', 'Perez', 40, 2500.00, 'Marketing')," >> /home/vagrant/datos_empleados.sql
    echo "('Lucia', 'Perez', 50, 2500.00, 'Ventas')," >> /home/vagrant/datos_empleados.sql
    echo "('Jorge', 'Perez', 80, 2500.00, 'Desarrollo')," >> /home/vagrant/datos_empleados.sql
    echo "('Miguel', 'Perez', 30, 2000.00, 'Ventas')," >> /home/vagrant/datos_empleados.sql
    echo "('Ruben', 'Perez', 70, 2500.00, 'Ventas')," >> /home/vagrant/datos_empleados.sql
    echo "('David', 'Perez', 30, 2500.00, 'Ventas')," >> /home/vagrant/datos_empleados.sql
    echo "('Olga', 'Perez', 30, 2500.00, 'Ventas')," >> /home/vagrant/datos_empleados.sql
  
  SHELL
end
