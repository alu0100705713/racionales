# Implementar en este fichero la clase para crear objetos racionales

require "./gcd.rb"

class Fraccion
  
  attr_reader :n, :d
  def initialize(n,d)  
    @n=n
    @d=d
  end
  
  def to_s    
   puts "La expresión es: #{@n}/#{@d}"
   a=gcd(@n,@d)
   puts "La expresión en su mínima expresión es: #{@n/a}/#{@d/a}"      
  end
  
  def *(other)
    Fraccion.new(@n*other.n,@d*other.d)
  end
  
  def entre(other)
  Fraccion.new(@n*other.d,@d*other.n)
  end

  
end

p1=Fraccion.new(10,3)
p2=Fraccion.new(40,2)
p3=p1*p2
p1.to_s
p2.to_s
p3.to_s
