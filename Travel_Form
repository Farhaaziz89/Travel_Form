import javax.swing.*;
import java.awt.*;

public class TravelForm extends JFrame {
    JLabel nameLabel, ageLabel, genderLabel, destinationLabel;
    JTextField nameTextField, ageTextField;
    JComboBox<String> genderComboBox, destinationComboBox;
    JButton submitButton;

    public TravelForm() {
        createAndShowGUI();
    }

    private void createAndShowGUI() {
        setTitle("Travel Form");
        setLayout(new FlowLayout(FlowLayout.CENTER));
        initComponents();
        setSize(300, 200);
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        setLocationRelativeTo(null); // Center on screen
        setVisible(true);
    }

    private void initComponents() {
        nameLabel = new JLabel("Name:");
        ageLabel = new JLabel("Age:");
        genderLabel = new JLabel("Gender:");
        destinationLabel = new JLabel("Destination:");

        nameTextField = new JTextField(20);
        ageTextField = new JTextField(20);

        String[] genders = {"Male", "Female", "Other"};
        genderComboBox = new JComboBox<>(genders);

        String[] destinations = {"Paris", "New York", "Sydney", "Tokyo"};
        destinationComboBox = new JComboBox<>(destinations);

        submitButton = new JButton("Submit");
        submitButton.addActionListener(e -> submitForm());

        add(nameLabel);
        add(nameTextField);
        add(ageLabel);
        add(ageTextField);
        add(genderLabel);
        add(genderComboBox);
        add(destinationLabel);
        add(destinationComboBox);
        add(submitButton);
    }

    private void submitForm() {
        String name = nameTextField.getText();
        String age = ageTextField.getText();
        String gender = (String) genderComboBox.getSelectedItem();
        String destination = (String) destinationComboBox.getSelectedItem();
        
        
    JOptionPane.showMessageDialog(this, "Submission Successful!\n" +
                "Name: " + name + "\nAge: " + age + "\nGender: " + gender + "\nDestination: " + destination);
    }

    public static void main(String[] args) {
        SwingUtilities.invokeLater(TravelForm::new);
    }
}
