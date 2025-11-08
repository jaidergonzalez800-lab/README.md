public class HojaDeVida {

    // Atributos
    private String nombreCompleto;
    private String correoElectronico;
    private String[] formacionAcademica;
    private String[] habilidades;

    // Constructor con tus datos
    public HojaDeVida() {
        this.nombreCompleto = "Jaider Fernando González ardila ";
        this.correoElectronico = "jaidergonzalez800@gmail.com ";

        this.formacionAcademica = new String[] {
            "Tecnologo"
        };

        this.habilidades = new String[] {
            "Bueno trabajando en equipo",
            "Bueno con las matemáticas"
        };
    }

    // Método para mostrar la hoja de vida
    public void mostrarHojaDeVida() {
        System.out.println("=====================================");
        System.out.println("          MI HOJA DE VIDA");
        System.out.println("=====================================");
        System.out.println("Nombre completo: " + nombreCompleto);
        System.out.println("Correo electrónico: " + correoElectronico);

        System.out.println("\nFormación Académica:");
        for (String formacion : formacionAcademica) {
            System.out.println("- " + formacion);
        }

        System.out.println("\nHabilidades:");
        for (String habilidad : habilidades) {
            System.out.println("- " + habilidad);
        }

        System.out.println("=====================================");
    }

    // Método principal para ejecutar el programa
    public static void main(String[] args) {
        HojaDeVida miHoja = new HojaDeVida();
        miHoja.mostrarHojaDeVida();
    }
}
