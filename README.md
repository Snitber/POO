
            this.titular = titular;
        } else 



       
        
        
        CASO B

    public class Principal {
    
    public static void main(String[] args) {
        // Crear producto con el constructor por defecto
        Producto p1 = new Producto();
        System.out.println("=== Producto por defecto ===");
        System.out.println(p1);

        // Crear producto con datos personalizados
        Producto p2 = new Producto("A123", "Mouse inalámbrico", 3, 45000);
        System.out.println("\n=== Producto parametrizado ===");
        System.out.println(p2);

        // Calcular subtotal
        System.out.println("\nSubtotal actual: $" + p2.calcularSubtotal());

        // Aplicar descuento del 15%
        double precioConDescuento = p2.aplicarDescuento(15);
        System.out.println("Subtotal con 15% de descuento: $" + precioConDescuento);

        // Incrementar cantidad
        p2.incrementarCantidad(2);

        // Mostrar datos actualizados
        System.out.println("\n=== Producto actualizado ===");
        System.out.println(p2);

        // Intentar descuento inválido (ejemplo)
        double descuentoInvalido = p2.aplicarDescuento(80);
        System.out.println("Intento de descuento inválido (80%): $" + descuentoInvalido);
    }
}
